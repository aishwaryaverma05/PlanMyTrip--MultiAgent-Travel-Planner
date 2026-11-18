Today's objective: Understand what an AI Agent is, how it works, and how it differs from a normal LLM call.

Task 1 — Understand LLM
45 min

Learn:
- What is an LLM? ans. LLM(large language model ek base model ki tarah act krta hai jo ki bahut hi huge dataset ke uper trained kra jata hai so that it can generate answer like human language.
- How does an LLM process input?  ans. llm direct hamara input process nhi krta ; process krne ke liye usko kuch steps krne hote hai like: (1)User i/p: user se i/p mangega (2) Tokenisation: words ko token m todega (3)EMbedding: ab token ko convert krdega numerical vector m (4)positional number: words different position m reh kr alag alag meaning bana skte hai toh usse bachne ke liye position mentaion krdeta hai llm (5) Transformer layer: yeh i/p ab process hokr transformer m jata hai [self attention ke paas phle jaha saare imp words extract hote hai then feed forward NN m jate hai imp words and process hote hai]  (6)then apko reponse generate hokr milta hai 
- How does it generate responses? and. same as above then jo bhi reponse high probab ka hota hai llm usko return krdeta hai 
- What are tokens and context windows? ans. tokens ka small unit of sentence ya para and context window is the max size of the info that llm can process ek baar m 
- What are system prompts and user prompts?  ans. prompts are instruction jo hum AI ko dete hai batane ke liye ki usko kya krna hai aur kya nhi : system prompt: is instruction jo hum ai ko dete hai btane ke liye ki usko kya krna hai [ex: act as ai engineer answer the following], user prompt: vo prompt hai jism hum puchte hai jo humko puchna hota hai [ex: what is xyz]

---------------------------------------------------------------------------------------------------------------

Task 2 — Understand AI Agent
60 min

Learn:
- What is an AI Agent?  ans. yeh ek aisa system hota hai jism hum apna goal dete hai toh yeh system uss goal ko padhta hai,smjhta hai , action krta hai vese jisse vo gaol pura ho sake and human ka role ek dum minimum ho 
- Main components of an agent. ans. 5 component hote : (1) perception: phle vo smjhega ki apne kya input diya hai (2) brainstroming: vo then sochega ki iss input m kya kya krna hai (3) Planning: ai agent then plan krega ki ab kya kya kese kese krna hai (4) tools/actions: then vo action lega task ko pura krne ke liye (5)then vo info store krega aur dega humko 
- How an agent receives a task.
- How it decides the next action.
- How it uses an LLM to make decisions.
