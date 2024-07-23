## Contributing Datasets

If you or your organization have datasets, which you would like to distribute
via our portal, please contact us via
[comunda-ops@googlegroups.com](mailto:comunda-ops@googlegroups.com).
Our process to publish a new dataset requires a number of steps:

1. Create an account on COMUNDA if you do not have one yet
2. Write a Data Use Agreement (DUA) that incorporates usage
   requirements that outlines acceptable use of your dataset by
   researchers.
3. Write to 
   [comunda-ops@googlegroups.com](mailto:comunda-ops@googlegroups.com)
   with a request to allow COMUNDA to publish your datasets. In this
   E-Mail:
   * provide the DUA you intend to use
   * specify if you want COMUNDA to
   host your datasets or just to host the datasets' metadata.
   * specify who should approve requests for dataset access - someone at your organization or
   COMUNDA staff
4. Once your contributor account is approved (this may take several days), 
   [submit a new dataset publication request](https://comunda.isi.edu/contributeDatasets)
   through the COMUNDA portal.  Be ready to answer the metadata questions
   listed below.  Once submitted, a dataset's record should appear online within an hour.
5. Once published, if your organization requested to handle dataset requests, please
   attend to them promptly. 
   Notifications will be sent to approving parties via E-Mail.

### Request Approvals

Data providers will typically approve requests for data sharing, but COMUNDA staff is willing to
take over data approver role or to help in vetting researchers, if you request this. An approver
will receive automated emails containing the signed DUA, and details about the requesting party's
name, affiliation and intended use of data. Data providers can request additonal information about 
requesting parties, such as citizenship. An approver approves or denies data access request. 
Providers can decide what their
criteria is for approval, such as whether to allow access only from
certain regions, or only from university faculty appointments, etc.
If approved,
data access will be provisioned to the requesting party, usually via direct email from the approver.
The provisioning process is only automated if COMUNDA hosts your dataset and you opted for download 
access mechanism. Otherwise, the approver must manually email the requesting party with dataset access
instructions.

### Hosting Datasets

COMUNDA will typically only host your dataset's metadata (title,
description, etc) while the actual dataset remains with you. COMUNDA we can also host your entire dataset in
addition to its metadata if you request this.

### Provisioning Data Acccess

Currently we support three types of data access:

* download - the researcher will obtain a link from request approver to download
  the dataset.
* onsite - the researcher will obtain login credentials for a system
  that has access to the dataset.  This is usually at the data
  provider's site.
* cloud - the researcher will obtain information about how to access
  the dataset within a public cloud provider's infrastructure.


## Dataset Metadata Expected During Submission

The following lists the fields that must be filled out during new dataset
submission:

- dataset name: a short name for the dataset
- brief description: a short sentence or two describing the dataset
- detailed description: a paragraph that describes the dataset and how it was collected
- the dataset "class": describing if the dataset is restricted, quasi-restricted, classified, or unclassified. This field has only internal use. If you want to vet researchers and then provide access to those you approve of, you would choose quasi-restricted.
- commercial use: whether the dataset can be used for commercial
  purposes
- publication review requirements: whether any publications making use
  of the dataset must be reviewed by the dataset provider before
  publication.
- availability: when did the dataset become available, and when does
  access cease
- in progress: whether or not the dataset is part of an ongoing,
  continually updating collection or whether collection has ended
- collection date ranges: when the collection start and stop
- dataset size: what is the size of the dataset in question
- indefinite use: whether or not the dataset can be retained and used
  indefinitely
- keywords: what keywords would be useful for helping researchers find
  your dataset
- format: what format is your dataset stored in? 
- anonymization: was the dataset anonymized in some way and how
- access type: how can the data be accessed upon approval (https,
  rsync, google BigQuery, or other)
- provider name: The name of the providing entity
- access duration: once approved, how long will the user be able to
  access the dataset
- Grouping ID: if the dataset is part of ongoing collection and you plan to publish
snapshots of the collection periodically, please use this field to "group" all datasets
in the collection together
- Data Use Agreement: the DUA to be applied
- IRB required: whether or not an IRB approval is required for use. We expect that fully anonymized datasets will not
require IRB approval, while those that are not anonymized may require IRB approval. If you select this field, researchers
will have to ask for and obtain an IRB approval from their organization **before** they can request your dataset
- Link to dataset: whether the data will be downloadable or will
  require on-site access with an account
- README: a markdown, text or html README file that fully describes
  the dataset.  Note that this will be converted to text when archived
  in the COMUNDA catalog -- fancy formatting is not possible at this
  time.


