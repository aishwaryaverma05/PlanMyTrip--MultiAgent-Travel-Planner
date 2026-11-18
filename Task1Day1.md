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
- How an agent receives a task. ans. agent ko task user se ya application ke through milta hai 
- How it decides the next action.  ans. agent next action resources , environment and current situaion ko dekhkr leta hai
- How it uses an LLM to make decisions. ans. it gives all the nescessary things the proj needs from llm.

------------------------------------------------------------------------------------------------------------------------

Task 3 — LLM vs AI Agent
45 min

Understand:
- Normal LLM call vs agent execution.  ans: llm call m sirf llm i/p ka answer generate kr ke humko deta hai normally , agent execution m llm i/p ko leta toh hai + generate bhi krta hai reponse aur aage ke actions bhi perform krta hai 
- Fixed response generation(llm call) vs multi-step task execution. (agent execution)
- Why an LLM alone is not automatically an agent. ans. as LLm sirf i/p leke generate kr skta hai response uske andr capabilities nhi hai of thinking and taking actions
- When an agent is actually required. ans. when the task requires dynamic decisions, actions and possibly multiple steps to achieve a goal.

------------------------------------------------------------------------------------------------------------------------


Task 4 — Tools and Tool Calling
60 min

Learn:
- What is a tool? ans. external func ya services hoti hai jo ai agent call krta hai jb llm vo kaam nhi kr pata ; ai agent kaam bolega llm ko [what is the weather in bhopal] then llm weather tool ko call krega [tool weather api se data fetch krega] then tool return answer to llm then llm gives answer
- Why do agents need tools? ans. tools external system ke saath interact kr skte hai isliye 
- What is function/tool calling? ans. llm decides which tool to call and what action to take 
- How does an LLM request a tool? ans. structured tool call request generate krta hai 
- Who actually executes the tool? ans. application ka code execute krta hai ; llm bas tool call request krta h
- How does the tool result return to the LLM? ans. tool result application ko deti hai and app. llm ko deta hai 


------------------------------------------------------------------------------------------------------------------------


Task 5 — Agent Decision Process
45 min

Understand:
- How an agent selects a tool. ans. agents randomly select nhi krta tool, user ki queries + jo tool available hai usko dekhkr tool select krta hai 
- How it uses tool results. ans. agents gets the result, agent dekhte hai ki result relevant hai? and decide krta hai aage actions ke liye 
- What happens if a tool fails. ans. vo retry kr skta hai agr temporary fail hai toh or altervative tool select kr skta hai or simple bol skta hai ki nhi retreive kr payega
- How an agent decides whether to continue or finish. ans . if the desired o/p is received toh continue
