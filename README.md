[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13164471&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

An important part of isomorphism is to have $(u,v) \in E_1$. In a completely connected graph every pair of nodes is connected by and edge so we can pick any edge $(u,v)$ in graph A and it will exsit in $E_1$. The same goes for graph B. 

Since graphs A and B have the same number of nodes and are completely connected we can say that the following situation exists. Every node in $V_2$ must have a corresponding node in $V_1$. Therefore there exists an edge $(x, y) \in E_2$ there is corresponding edge $(f^-1(x), f^-1(y)) \in E_1$. Each node in graph A maps to every node in graph B which fufills the requirements for an onto function.  

Finally, because the two graphs have the same number of nodes we can say that the following situation exists. Each individual node in $V_1$ must map to a distinct node in $V_2$ For every node, any edge $(u, v) \in E_1$ there exists a corresponding edge $(f(u), f(v)) \in E_2$ and vice versa. Each node in $V_1$ is uniquely mapped to a node in $V_2$ and vice versa. This meets the requirements for an one-to-one function. 
 