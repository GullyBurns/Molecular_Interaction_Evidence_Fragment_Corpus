# Intact Evidence Fragment

## Basic Premise

'Evidence fragments' are the text elements of a scientific paper that specifically describes the evidence presented in figures to statements about their scientific meaning. We here describe a corpus of fragments derived from papers concerned with molecular interaction experiments (curated into `Pathway Logic` or  `INTACT`). All literature-based data is derived from open access papers.

## Curation Guidelines

1. Only curate paragraphs from the results sections of primary experimental papers (i.e., papers where original experimental research was performed).
2. Tag each high-level clause with one of 7 codes: `none`, `hypothesis`, `problem`, `goal`, `method`, `result`, `implication` (derived from http://arxiv.org/abs/1702.05398).
3. For any clause, associate them with a figure or a subfigure.  
	* Use codes like `f1a`, `f1b`, etc to link to subfigures
	* Use whole numbers to link to figures without subfigures or all aggregated subfigures in a given panel. 
	* Do not link information intended as background (i.e, that cites other papers).
	* If a clause cites (data not shown), link it to `uX` (where X is a number).
	* If a clause includes more than one figure use a pipe separator: e.g, `f1a|f1b`

## Repository organization

The subdirectories of this directory are organized as follows.

* 00_uncurated - TSV files to be processed* 01_discourse_tags_complete - TSV files where all discourse tags are included* 02_expt_spans_complete - TSV files where all discourse tags and figure columns are included* 03_primary_claims_complete - TSV files where all discourse tags, figure columns, and checks for primary statements are included

