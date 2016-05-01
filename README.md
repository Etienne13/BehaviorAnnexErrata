## Synopsis

This project aims at sharing the AADL Behavior Annex Errata in order
to have the AADL committee members syncrhonized on discussions,
proposed resolutions, and status of Errata. The remainder of this
readme file describes the content of this repository, and explains how
to submit new errata, discuss existing errata, and follow the
evolution of existing errata.

## Structure of the repository

The repository is organized as follows: 

- version X.Y is a directory that contains, in a single file, a
description of a set of modifications that were adopted by the
committee in order to produce release X.Y of the Behavior Annex
document.

- adopted is a directory that contains a set of documents. Each
  document is a description of an adopted erratum with the initial
  rationale of the erratum, a description of the erratum, a
  description of the adopted resolution, and an illustrative
  example. The adopted resolution must refer the version of the
  document to which it applies.

- rejected is a directory that contains a set of documents. Each
  document is a description of a rejected erratum with the initial
  rationale of the erratum, a desription of the erratum, and the
  reasons for its rejection.

- submitted is a directory that contains a set of documents. Each
  document is a description of a submitted erratum with the initial
  rationale of the erratum, a desription of the erratum, and the
  version of the document on which it is applied.

- meetings_history is a directory that contains all the slides
  presented to the AADL committee meetings.

## Life-cycle of errata

Before all, make your own fork of the repository.

1) The first step of the process is to submit new errata. To do so, copy
in a new file the template provided in directory "submitted". 

This new file is the errata you plan to submit. Its name must start
with the errata identifier, with the following form: SEC.ID_NB.KW
where SEC is the identifier of the section of BA to which the erratum
applies, and ID_NB is an integer value that identifies the erratum,
and KW is a very short keyword to reference the erratum.

Fill the different sections of the template to describe the
errata. Add, commit, and push this new file to your repository. Once
this is done, ask for a merge request with the initial repository.

Note that the template is provided as a word document, but you can use
any format as long as it is "easy to open (does not depend on
proprietary tools)" and as long as it contains all the sections of the
proposed template.

2) Errata dicsussions should be done using the github interface via
issues. These discussions can then be used during committee meetings
to start discussions and make decisions.

3) During meetings, errata are further discussed, and decisions are
made: rejection, adoption, or delay. If delayed, the file describing
the erratum remains as it is until a decision can be made. If adopted,
the file describing the erratum is moved to the adopted directory and
the resolution is added to the description of adopted modifications in
directory X.Y. If rejected, the file describing the erratum is moved
to the rejected directory and the reasons for the rejection are added
in the file.

