This repository demonstrates the integration of a [Discourse Graph](https://discoursegraphs.com/) layer to enhance research ideation and synthesis for an HCI researcher.
## What the Discourse Graph layer adds and how

The Discourse Graph is a simple information model of scientific argumentation and processes, that describes how **Experiments** are motivated by the desire to answer or inform scientific unknowns (**Questions**) with generalizable **Claims** (or conclusions or hypotheses) that are justified by sufficient empirical **Evidence**. 
![](Discourse%20Graph%20model.png)

This model is easily adapted to cover the kinds of questions and contributions that constitute research in Human-Computer Interaction (HCI). For instance, we can add DG nodes for Patterns and Artifacts to help structure work on contributing new Design Patterns (instantiated in specific Artifacts that we can test and explore) to address "How might we" research problems in HCI. The following figure shows the updated model:

![[Discourse Graph  model (HCI).png]]

This model can help structure synthesizing new HCI research directions in close conversation with existing/prior work.

For example, if we're making a systems contribution, we can review the design space / history of prior art we build on and/or contribute to, w/ something like the following structure
- For each key [[PTN]]
	- Describe key exemplar [[ART]]s for this [[PTN]]
	- Key [[CLM]] and [[EVD]] about this [[PTN]] in relation to our core problem
	- And any open [[QUE]] we address
		- e.g., does [[PTN]] work for our task? what might the [[ART]] look like?
		- [[ART]] seems awesome, but doesn't quite do X, how do we make it do x
		- lots of people say [[PTN]] is great, but we don't have great [[EVD]] that it actually works

Or if we're making an empirical contribution, we can review prior insights and questions we build on and/or contribute to, w/ something like the following structure
- Key [[CLM]] about some core (sub)[[QUE]]
	- Key supporting and opposing (possibly conflicting!) [[EVD]], with intuitions about strength of [[EVD]]
	- And then any open [[QUE]] that remain that we address
		- e.g., [[CLM]] is big if true, but we really don't have good [[EVD]] for it (for our context, or bc the methods suck for XYZ reasons, etc.)
		- [[CLM]] A and [[CLM]] B are in major tension, here's what a decisive [[EVD]] would look like that arbitrates between them

The Discourse Graph model can also support new workflows that **enhance synthesis and coordination for ongoing research projects**:
1. **Marking potentially significant observations** that could be the basis of empirical evidence or artifacts to share, without breaking the flow of the day to day work of documenting procedures and observations in the notebook.
2. **Revisiting potentially significant observations and [formalizing](https://discoursegraphs.com/docs/obsidian/creating-discourse-nodes) them into discrete "micropublications"** to support within-team sensemaking.
3. **Gathering and visually synthesizing discrete  micropublications** into a scientific or design argument to support reflection and planning of next steps. This can be done via a mixture of [creating discourse relations](https://discoursegraphs.com/docs/obsidian/creating-discourse-relationships) between nodes and mapping nodes on a [discourse canvas](https://discoursegraphs.com/docs/obsidian/canvas).

These workflows are designed to add to, rather than detract from or materially change, the existing workflows here of documenting observations in the experiment/design logs, archiving code and data for sharing, and so on.
## Some technical details and how to try

To try out this vault, simply download the vault (via git or zip), open Obsidian, and open this directory as a a vault in Obsidian.
### Folder structure and new files
TODO.
## Plugins
The vault also includes the following plugins to support the above workflows. Since the vault includes the `.obsidian/` files, these plugins and their settings are already set up.
### Core plugins
- `Bases` for easy querying of Discourse Graph nodes
### Community plugins
- Core functionality
	- `Discourse Graph` - enacts the main workflows for documenting and formalizing discrete empirical observations described above
	- `Datacore` - dependency for `Discourse Graph`
	- `BRAT` - dependency for `Discourse Graph` and `Datacore`
- QOL
	- `Better Search Views` - easier exploration of candidate nodes, with more context
	- `Copy Block Link`- easier linking to specific spots in the notebook, esp. ones that contain candidate DG nodes
	- `Better Search Views`- came with the example vault
	- `Natural Language Dates`- nice to have


