# Learning About Causal Systems Through Play

Sim, Z., Mahal, K. & Xu, F. (2017) Berkeley Early Learning Lab  
Keywords: free play; causal learning; generalization

## Study

Data analysis to show that children are able to learn more complex causal rules through free play. 

Children and put different blocks on machines to make the machine go (play music). Blocks and machines have various shapes and colors, so do they learn the rule faster through free play? 

The paper containing study design and method can be founds [here](http://docs.wixstatic.com/ugd/9f32e5_2732ecc1ff134ea299b72f1316a7bf9b.pdf).  

### Purpose

Code children's choice of machines and blocks to learning outcome, according to how similar they are to the correct rule. Then compare the learning outcome of free play and didactic learning.

<p><img src="https://raw.githubusercontent.com/lizzij/DDAF/master/freePlayMaterial.png" width="500" align="middle"></p>

Rules are:
* Number rule (number of blocks per machine);
* Shape match (between blocks, and between block and machine);
* Color match (between blocks, and between block and machine);

Coding scheme (sum of):
* Number rule concurrence;
* Block-block rule concurrence divided by # of relation(s);
* Block-machine rule concurrence divided by # of relation(s);

## Usage

For instance, this is a an example of one choice of machines and blocks: 

```
BR1::pR&rR:::BR2::rC&pT&pC
```
Denotes: 
* the child pick up "1 blue rectangle machine" and 
* put "1 purple rectangle block + 1 red rectangle block" on top of it; then 
* the child stacked "1 blue rectangle machine" and 
* put "1 red circle block + 1 purple triangle block + 1 purple circle" on top of it; 

The coding scheme returns:
```
0 + 0.75 + 0.5 = 1.25
```
### Setup

Install openpyxl:

```
$ pip install openpyxl
```
