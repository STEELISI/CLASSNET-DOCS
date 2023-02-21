## Correcting and Sharing Labels

Some datasets in our collections are labeled with security-relevand and/or
network/relevant labels (e.g., "benign", "attack", etc.) In some cases
researchers may want to offer a correction to our official label, or a new way
to assign labels, or even
to propose a new set of labels to denote new features of flows, hosts or events. Please follow the instructions below to correct or share labels.

### Correcting a Few Labels

You can make corrections by interacting with Github or by giving us a URL with the corrected labels.

#### Github interaction

* Check out the public repository for labels:
```
git clone https://github.com/STEELISI/COMUNDA.git
```
* Find the folder where the affected dataset is, and then find the folder
where our official labels reside
* Fork a new branch:
```
git checkout -b your-chosen-name
```
* Apply your changes
* Commit and push
```
git commit -a -m 'some message here' && git push origin your-chosen-name
```
* Go to [COMUNDA Github](https://github.com/STEELISI/COMUNDA) and submit a pull request. Make
sure to offer a detailed explanation in your request about the reasoning
for the corrections you suggested.

#### Giving us a URL

On [COMUNDA Web page](https://comunda.isi.edu) log in and then follow *Update Labels* link on
the left. This will enable you to provide us a URL with materials describing your label correction.
Please make sure to provide at the URL site:

* Reason for correction
* File with corrected labels and unique record IDs (ideally corrected labels would be in the format that the original labels were)


### Share New Labels

You can make corrections by interacting with Github or by giving us a URL with the new labels.

#### Github interaction

* Check out the public repository for labels:
```
git clone https://github.com/STEELISI/COMUNDA.git
```
* Find the folder where the affected dataset is, and cd into it

* Fork a new branch:
```
git checkout -b your-chosen-name
```

* Create a new folder
for your labels. Name that folder in a way that denotes your or your research
group's identity and the purpose of the labels, e.g., JMirkovic-ddos-attack
* Place the following information and files into the folder:

  * Your name and contact information in README.md file
  * The label format in README.md file. Make sure to explain each label's meaning.
  * The label file if any (sometimes the labeling program may take input needed to label, without the label file)
  * The program, which can be ran on the given dataset to produce some unique record ID and the desired label. This program may take input from command line or take label file as input.
  * Provide examples how to run the program (and specific inputs) to label the given dataset

For example, if I were to label DDoS attacks on the large dataset containing Netflow records, I may choose to have labels in the format of attack events, e.g., start time of attack in UTC, stop time of attack in UTC, target, type of attack or attack traffic's signature, I would specify this format in the README.md file, and list the types of attacks I can label. I would place the events into the label file. I would also provide a program, which reads Netflow records and my label file, and prints a unique record ID (timestamp-sourceIP-sourceport-destIP-destport) and the label out. I would put the full example of the command line needed to run my program in README.md

* Commit and push
```
git commit -a -m 'some message here' && git push origin your-chosen-name
```
* Go to [COMUNDA Github](https://github.com/STEELISI/COMUNDA) and submit a pull request. Make
sure to offer a detailed explanation in your request about the reasoning
for the labels you suggested and the labeling algorithm you implemented.

#### Giving us a URL

On [COMUNDA Web page](https://comunda.isi.edu) log in and then follow *Update Labels* link on
the left. This will enable you to provide us a URL with materials describing your new labels.
Please make sure to provide at the URL site:

  * Your name and contact information in README.md file
  * The label format in README.md file. Make sure to explain each label's meaning.
  * The label file if any (sometimes the labeling program may take input needed to label, without the label file)
  * The program, which can be ran on the given dataset to produce some unique record ID and the desired label. This program may take input from command line or take label file as input. If label file lists each record's unique ID and the label, then the program can be omitted.
  * Provide examples how to run the program (and specific inputs) to label the given dataset. Again, if label file fully specifies the label for each record, the examples can be omitted

