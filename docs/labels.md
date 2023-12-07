## Viewing, Sharing and Collaborating with Dataset Labels

Some datasets in our collections are already labeled with
security-specific and/or other relevant labels that offer insight into
each record within a dataset (e.g., "benign", "attack", etc.)
Researchers may want to contribute their own labels, either as an
alternative to any existing labels or to create entirely new labels
denoting new features of flows, hosts, records or events.  Finally, if
you believe that the existing labels are in error or could be
improved, feel free to submit a request to update the existing set of
labels as well.

To add your contributions to the existing set of labels for a dataset,
please follow the instructions below to share labels.

### Viewing the labels

The labels for all datasets currently exist within a single GitHub
repository.  To view and work with them, you will need access to the
dataset itself (or else the labels will have little value) and the
label repository as well.  To get the label repository, download the
repository from github:

    git clone https://github.com/STEELISI/COMUNDA.git
    
### Correcting existing labels

You can offer corrections to the existing labels using GitHub pull
requests or by sending us a URL with your corrected labels.

#### Creating Github Pull Requests

* Begin by forking the main repository on github using the `Fork`
  button on the website for the COMUNDA repository:

     https://github.com/STEELISI/COMUNDA.git

* Then clone (check out) your fork: 

    git clone https://github.com/YOURACCOUNT/COMUNDA.git

* Find the folder where the dataset you wish to offer corrections for
is, and within that find the folder where our official labels reside
* Create a `git` branch to save your changes in:

    git checkout -b your-chosen-name

* Mark (add) any changed files you wish to submit for inclusion

    git add [changed-files]

* Commit and push

    git commit -m 'some message here'
    git push origin your-chosen-name

* Finally, go to [COMUNDA Github](https://github.com/STEELISI/COMUNDA)
and submit a pull request referencing the branch that you just pushed
to your own forked copy.  Make sure to provide a detailed explanation
in your request about why you are suggesting the corrections you made.

#### Sending us a URL of changes

Alternatively, if you are unfamiliar with using git and GitHub, you
may send us a request via the COMUNDA interface.  On the [COMUNDA Web
page](https://comunda.isi.edu) log in and then click on the *Label
Datasets* link on the left. This will enable you to provide us a URL
with the materials and changes that describe your label correction.
Please make sure to provide:

* Your reasoning for the  correction
* A file with corrected labels and unique record IDs (ideally
  corrected labels would be in the format that the original labels)

### Share New Labels

For creating new labels, use the same process as described in the
above instructions for correcting labels.  But, instead of modifying
existing files, create an entirely new folder instead for your newly
created labels.  Name this new folder in a way that denotes your or
your research group's identity and the purpose of the labels (e.g.,
JMirkovic-ddos-attack).

Place the following information and files into the folder:

* In a `README.md` file include:
    * your name and contact information.
    * The label format used in your labeling files. Make sure to
      explain the meaning and purpose for each label.
* The labels you want to contribute either in the form of a file
  containing the labels, or as a program or script to execute for
  generating the labels given the dataset files.
* Provide instructions and/or examples how to use the labels or run
  your program or script and the inputs it needs.

Finally, push your forked GitHub branch to github (`git push origin
your-chosen-name`) and then create a pull request at [COMUNDA
Github](https://github.com/STEELISI/COMUNDA) as described above.  Make
sure to offer a detailed explanation in your request about the
reasoning for the labels you suggested and the labeling algorithm you
implemented.

##### Example scenario

For example, if I were to label DDoS attacks on a large dataset
containing Netflow records, I may choose to have labels in the format
of attack events that include the start time of attack (in UTC), the
stop time of attack, the target, the type of attack or the attack
traffic's signature. I would specify the format of any files
containing this information in a newly created `README.md` file, along
with any other pertinent information. I would then place the events
into a label file (potentially a CSV, JSON or tab-separated format). I
might also provide a program or script to read the Netflow records and
create a label file that's output would include a unique record ID
(for example timestamp,sourceIP,sourceport,destIP,destport) and an
associated label (e.g. "attack" or "ddos"). I would put the full
example of the command line needed for running my program in the
`README.md` file.

#### Sending us a URL

You may also send us a URL containing all of the information needed
for a new set of dataset labels.

To do so, log into the [COMUNDA Web page](https://comunda.isi.edu) and
click on the *Label Datasets* link on the left-hand side. This will
provide you a form to fill out with a URL pointing to your materials
to download, and a textbox to please a description in that describes
your proposed labels.  Like the above, please provide:

* In a `README.md` file include:
    * your name and contact information.
    * The label format used in your labeling files. Make sure to
      explain the meaning and purpose for each label.
* The labels you want to contribute either in the form of a file
  containing the labels, or as a program or script to execute for
  generating the labels given the dataset files.
* Provide instructions and/or examples how to use the labels or run
  your program or script and the inputs it needs.


