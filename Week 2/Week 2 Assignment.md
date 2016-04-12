##Nearsoft Academy
**Week # 2**  
**Code Jam (3 Problems)**  
**Video Reviews (11)**  
**Cesar Dario Garcia Jimenez (Internship)**  
**cgarcia@nearsoft.com**  

****************************************************************************************************************

##Video No.1  

##“The Myth of the Genius Programmer”  
(by Brian Fitzpatrick and  Ben Collins-Sussman at Google I/O 2009)    
    

This presentation speaks up things that a lot of people think and feel but not many talks openly about it in professional environments, this presentation speaks of how insecurity in professional environments affects performance. Software developers are humans and we may feel insecure about our performance in work from time to time, and it is natural and it is OK.
Sometimes inside the software developer groups can exist different behaviors like elitism or being territorial about someone's code and this commonly leads organizations to be unhealthy and to have insecure or unhappy people inside of it, software developers are people and people often will learn, think and feel different from each other and also people have different skills and weaknesses, and they may grow up in different directions at different speed and perhaps in a different time.
Insecurity is a performance enemy, it inhibits personal and professional progress as it builds a barrier between team members where effective feedback and support is sacrificed.
When software developers feel insecure about their code or performance at work when faces others that are more skilled or experienced, and insecurity may lead to developers to feel really bad about showing their work to others and specially about showing their mistakes.
We are recommended to be more open to show our code and work and to maintain an open door to critics, advices and all the feedback we can get, code reviews is an example of an excellent exercise to learn new things, be ready to accept any kind of feedback and learn from it and if you fail at something learn from it too, and do things differently next time.


##Video No.2  
  
##“#perfmatters: Tooling techniques for the performance ninja ”  
(by Colt McAnlis  at Chrome Dev Summit on 2013)    
  
Colt McAnlis exposes why performance in Mobile and Web development matters (a lot).
Internet has come to revolutionize almost every aspect of human life, it has change the way we communicate, and among other things, it has come to change the way we do business. People understood that the reach of the Internet can make your business be reachable for almost every place in the world, so almost every business has created a website to provide information about their products or to sell something, and a lot of people are buying over there, that means websites represent money.
Now if you want to people to Brian Fitzpatrick, Ben Collins-Sussmanvisit your website, it has to be solid and it has to be fast because one of the biggest reasons for people to leave your website its because it is slow. When  Internet was born you can't t address this kind of problems but now we know because of the developer tools available to measure the speed and performance of your website/business over all different kind of devices that people use to connect, mobiles don't have the same power that laptops or computers so you have to focus on performance.
The Performance of your website matters, so how do you take it to the next level?, the first step is to find out how your website runs over different devices, you gather information and then you get insight of what is going on, when performance problems are address d you take action to solve it.

 “What you can measure, you can optimize”, Speed is essential, but you have to look under the bones of your design to get it right, your website loading time is a side effect of bad design under your website architecture “your website does not have a performance problem, but a plethora of performance problems”.  
  
There are 3 main pillars to focus on for performance improvement in order to get your website working over computers and specially over mobile devices:
Network: This translates as the time it takes for your website to load. From here derivate other two aspects.
Render: This is one of the main problems for achieving good performance on your mobile devices, render may demand resources that maybe are not suitable for small mobile devices and  you have to address that.
Compute: as in the the render pillar, technologies for processing your website demands resources that may show good performan12ce while testing your website over your laptop, but now that we can measure how well mobile devices runs the website, we find that of course, mobiles are not as powerful so if you want to deliver an successful experience over all devices you have to address the compute performance problem too.
  
The performance of your website is vital for success, each time a user leaves your website for not having good performance you losses money.
  
##Video No.3.1  
  
##“Variable Length Codes (Ep 1, Compressor Head) ”    
(by Colt McAnlis from Google Ddevelopers on 2014)    

  
As the Internet became more popular, people started to share gigantic amount of information, so in order to get this huge amount of information running over a limited set of resources computer scientist from late 70's have been utilizing compression to effectively reduce the size of this content and prevent the Internet from coming to a standstill.
Variable length codes is a method to reduce the amount of bits needed to transmit information, this takes us to encoding and decoding methods over data transmitions, for example in modern computation we use bytes to encode alphabets which is a fixed 8 bit pattern, this is nice but not optimum because maybe there are other ways to represent the same alphabet using variable length codes, now this represent a challenge because when you start creating your encoding method you start with only two values which are 0's and 1's, so if you want to represent a large alphabet you may have problems figuring out how to actually decrypt and know what letter you are sending, because it is common for a letter sequence to exists inside of another larger one, so how do you know when to decide what letter you are encoding and decoding.
This is where the entropy concept comes in, entropy stands for measuring the smallest amount of bits needed per average to represent your data stream using variable lengths according to the information theory and it makes use of statistics, you can calculate the entropy needed for your variable length data transmission algorithm by their appearance percentage rate, this derivate into several encoding techniques such as the use of prefixes.
  
Colt McAnlis explain us a really good example which are binary trees to represent letters organized hierarchically by their appearance percentage rate. 
  
This leave us with a good start to think about new methods for improve performance of our data transmissions using variable length codes. 
  

##Video No.3.2
  
##“The LZ77 Compression Family (Ep 2, Compressor Head)”    
(by Colt McAnlis from Google Ddevelopers on 2014)   
   
  
This videos reveal us the leading family in the data compression methods, The Lempel-Ziv family.  
  
The LZ77 compression family is an approach for finding the balance compression methods 
as such we know that not every data transform is suited for every type of data, so you  
have to know the data you are working with in order to find a valid transformation.
  
This family was born around the problem of finding the balance between finding the longest chains of characters and finding the lowest level of entropy, so we end up with dynamic grouping, which is not a easy task.
LZ77 is the best algorithm to find  the best optimal way to tokenize a string so for since no other algorithm created is able to beat the efficiency of LZ77. This algorithm consists in splitting the stream into two segments, left side called the “Search buffer” which are the tokens we already decode, and the right side called the “Look ahead” buffer which are the tokens we have not decode yet.
When the algorithm starts it try to find the longest known stream of symbols comparing it to our search buffer to find a match, the symbol stream is always divided into three parts (offset, length and the next token”), and when it finds a match it split the new stream, and stores it as a list [], and keeps running until finished, the objective is to end up with an array of lists and then follow their own associative lanes to create compression.
The LZ77 algorithm and another derivate called the LZ88 algorithm are the father of a family of derivate with slightly differences between them, and they are the responsible for many of the data compressors we use in present time like winzip, winrar and 7zip.
This is a very revealing story about data compression.

##Video No.3.3
  
##“Markov Chain Compression (Ep 3, Compressor Head) ”  
(by Colt McAnlis from Google Ddevelopers on 2014)    
  
  
Markov Chains Compression is the at the cutting edge of compression algorithms. These algorithms take makes use of artificial intelligence to compress by allowing the encoder and decoder to predict what data is coming next.
Markov found a new branch of probability, he becomes aware of a way of predicting the next symbol of a stream by giving each symbol a possibility for change into two more states by one way and then the ability to come back using a different way leaving us with 5 bits to represent the different states.
The algorithm works by splitting the symbols and creating and forming unrelated trees for each symbol using the next occurrences in the stream as the leaves of each symbol using a initial symbol as a initial state in automates theory, and then it goes forming trees or “lists” of possibilities, of course this leaves us with the probability of having to create some very big trees of probabilities, so how do we address this problem?, using the variable lengths algorithms, then we have to make use of statistics in order to organize our trees by appearance percentage. 
This is a very interesting algorithm to keep studying for a better comprehension because it is used in present time to predict all kind of things, not just for data compression.
  

##Video No.4
  
  
##“The Art of Organizational Manipulation”  
(by Brian Fitzpatrick and Ben Collins-Sussman on Google I/O,  2012)    
  
  
The presentations speaks of the possible perspective for a company to have:  
the real thing vs the ideal thing.
  
The ideal is to have a company full of leadership where everybody does what it has to do without having anyone behinds their asses, but of course this doesn't happened very frequently because in hierarchical organizations managers tend to avoid to delegate some important tasks and employees are not empowered to be responsible for themselves.
Companies should start working by a different paradigm if they want to get everybody as an auto motivated and empowered member that can be responsible for himself to move the company forward in their vision.
Trust is the key in here, it make members of an organization to start acting, they are empowered to do so and in a good and in a consciousness way. This is a difficult decision to make and the transition for a company to achieve a thing like this can be rough but it worth it.

##Video No.5
  
##“Programming Well with Others: Social Skills for Geeks”  
(by Brian Fitzpatrick and Ben Collins-Sussman on Google I/O,  2011)    

  
This presentation show us why it is important to develop soft skills for working in the Software Development industry, because hard skills are not sufficient if you want to achieve big things, because collaboration with others is key for that.
Inside of a company exists different kinds of members and as tools for developing software has evolved, the way of organizing people and the threat they receive is keeping organizations from having empowered and motivated members.
The way that an organization threats its members affects their personal motivation to grow professionally to push the company to bigger goals and that leave us with members that are static. Those members are always needed to tell to them what to do, they cant act or think how to get things better.
The presentation proposes to threat your employees different, motivate them to keep learning and push them to evolve into high valuable members that don't need to be told what to do next.


##Video No.6

  
##“Developing-Expertise”  
(by Dave Thomas on  2008)  
  
  
In this presentation  Dave Thomas talks about expanding people's expertise in their domains of interest by not treating them uniformly as they had the same amount of knowledge and level of experience.

The point on this talk is to make a point about how important is in the engineering also care about social aspect and not only on the technical abilities, specially when you are working on a team.
If you wanna be a successful engineer also have to focus on social, because companies are formed by people, and to reach success you have to do it in team, its gonna be extremely difficult to do it alone.
To start working on a team from the beginning of the project, you have to present the design, or a prototype and then collaborate, this if it is your idea, because otherwise if you try to build a team when you already have part of the project done, the other people maybe wont like to work on it because its already done.
In a group of people always someone amuses the role of leader, even if nobody assigned him that role, and this is not necessary a problem, the thing here is that that person realized he does not take decisions, but put order to the team.
To encourage people is better to give freedom to take decisions and not limit them, because is gonna be uncomfortable to work feeling this kind of pressure, that also limits creativity.
  
  
##Video No.7

##“CouchDB and Me”  
(by Damien Katz on  2009)    
    

This is the story of how couchDB was developed, told by his creator Damien Katz. CouchDB is an open source database that uses different technologies (JSON to store data, javascript as querys, http as an API).
  
Damien explains why he changed or was fired so many times from his job, and why he finally decided to sell all  he had and start working on his own project (CouchDB). 
uniformly as they had the same amount of knowledge and level of experience.
Damien's first thought were that he would like to work on a cool project, his job were something he would like to do. So, he sell his house and moved with his family to north Carolina and started living from their savings. Were times when he did not receive any incomes.
Then started thinking what to build and remembered an idea he was working since college and some other projects he worked before.
When he finally had the idea started thinking on how to build it. He felt frustration because he had no idea how even to start and felt panic.
The initial version was in C++, but as it was evolving it was changed. He had previous knowledges of Erlang he thought it was cool language, and compared to other languages, getting something working reliably was much easier and does not require much talent.
When the prototype was finished, he started looking for investors in 2007 when they were waiting for another baby. But he was not able to find any, and decide to accept a job in MySQL and for that time he stopped working on CouchDB.
Then he receive an email from IBM wanted to hire him. And they told him they were gonna paid him to continue developing CouchDB.


##Video No.8


##“Perfection is an unrealistic goal”  
(by Linda Rising on  2009)    
  

The challenge of being agile. The best way to work as an individuals. The main things I learned fro this talk is about the importance of working taking breaks each certain time. You become more productive when you work straight for like 90 min, and then take a 20 min break. This is because our brain is designed to work in cycles, and this happens both when we are asleep and when we are awake, working.
In this presentation Linda is explaining the moment when the mind is more active, and that we can perform a better work when we do it during this phase, and the importance of taking a break when your brain is not in this phase.
She states that sleep is divided into 90-minutes cycles:  
-Light sleep – muscle relaxation, slowed heart rate.  
-Completely sleep – metabolic levels are extremely low.  
-Delta – blood pressure rises, brain activity increases. Dreaming occurs,  
  
**Do we cycle in the daytime? **  
Humans move between expenditure of energy and renewal of energy all the day long, this is the cycle she is talking about. Establishing that rhythm we are more productive. And she says that is more important to manage your energy than your time.
We are more productive if we work per cycles instead of long times, and spend the time between these cycles taking breaks, relaxing or distracting the mind.
90 min is the optimum duration, but they notice that longer pair durations had higher mean velocities.
  
Also she states that a new research (back in 2007) states that neurons not necessary die as we get older. Regions of the brain can actually expand their complement of neurons as we age. 
  
The final quote she says is that perfection is in unrealistic. Improvement is more realistic (1% by the end of the next generation).


##Video No.9
  
##“The Power of an Agile Mindset”  
(by Linda Rising on 2015)    
  
  
Wonderful and motivating speech for those who think they can't do better, at any moment of your life, you can!!!.
  
In this speech Linda shares to us her encouraging story explaining that you can always be better but how is this possible?
    
It's all about your mindset, the way you think of yourself, your capabilities and your attitude. You may think that if you are not good at something since the beginning you are doomed to keep this way but that's not true at all, and you must change that way you think, you can always grow better no matter what (no matter age, no matter gender, no matter what others or even you think about yourself).
  
Linda tell us about a social experiment that shows how people with better attitude eventually succeed on their goals, they called this attitude as “Agile mindset”, Agile mindset is a state of mind where you believe in improving yourself, you believe in failure as an opportunity to learn and do things different next time, and you can.
  
**Agile Mindset vs Fixed Mindset:**
  
People may have the incorrect thought that says that “either you have it or not”, it means that people believe that their destiny and capabilities are limited and defined by circumstances, this wrong way of thinking is called the “Fixed Mindset” and you should stop thinking about yourself that way, all the people is different and have different capabilities, that's true, but if you think that it will always be that way you are believing a lie, you can always improve yourself, you can always learn from failures and do a better effort next time.

**It's all about Learning:**

I encourage you to start thinking differently about yourself, attitude and effort are keys for  getting results and it is all about learning.
  
Personally I feel very identified with what this video is about, I recognize that I used to be more on the side of the fixed-minded, but something happened, I am older than my student partners at university, I am less wealthier economically speaking than the people of my age, and I am not what I want to be or be where I want to be, but I decided to change that because I wanted to do what I do now, I decided that I can change and I'm doing better and better and I keep learning a lot of things that are making me better, and I know I will continue growing, I am not where I want to be, but I am making my way over, and you can definitely do it too.

##Video No.10
  
##“Collaboration, Bonobos and The Brain”  
(by Linda Rising on 2007)    

This presentation is an interview with Linda Rising, and she talks about behavioral patterns inside teams.
  
Linda tell us from its research over cognitive psychology that we tend to repeat patterns as we learned them from our experience over evolution and how them become hardwired into our brains, and since we know we are related to primates, we studied the behavior from our nearest related primate, which are chimpanzees or at least thats what we thought until now.
  
Chimpanzees have an aggressive and hierarchical structure so we used to think that it was natural to us to behave in the same way, but recent studies showed that we have another primate specie to be as nearest related to us as chimpanzees, this specie are the bonobos.
  
Bonobos behave completely different from chimpanzees, bonobos tend to be cooperative and  friendly with others, when they face a situation where competition can takes place, they perform rituals to release tension between each other and then they collaborate and celebrate together when they succeed the situation.
  
As to software development is concerned, it turns out that agile methodologies have shown to work because some of their principles assimilate to the bonobo behavioral patterns.For example people feels more comfortable by working in small groups because in that way rituals occur more easily and they can solve social tension better. We are proving that we can change our patterns, we can change our behavior to be different and it is making sense that by being cooperative and acting more like the bonobos we get better results.
  
This is one scientific aspect behind the success of Agile methodologies.
  

##Video No.11

##“Prejudices Can Alter Team Work”  
(by Linda Rising on 2008)  

  
Linda Rising has been studying the recent discoveries of a science called Cognitive Psychology which studies the ways we perceive and how we learn from reality and how this affect us and our societies, in this speech Linda talks about one specific aspect which are prejudices.
Judges are naturally for us because we 10have learned to evaluate “good” and “bad” things during our evolution as specie, it has helped us to survive at some point of our history, some of this judges comes from personal learning, others may come from our family or society, and many of this judges will be stored in memory and triggers each time we face a similar situation. 
The problem is that our brains judge automatically and in a unconscious way, and perhaps something learned in the past about some situation can be absolutely trivial while facing a similar situation during present, that is the problem with prejudges, we filter present through our personal learnings in the past. 
We are often driven wrongly by prejudges and this is a negative things for us, perceptions affect the way we relate to others and the way we relate to reality in general.
Another problem is when we are under prejudges from others or when we hold prejudges about ourselves, our performance is badly affected, it unconsciousness triggers insecurities in us and in that state we don't execute well, prejudges stops ourselves from perceiving reality as it is.
We must make an active effort to realize if our thoughts are well based on a present situation, and further more we have to look for the better, if we work to develop a positive perspective we will affect us and our environment in a very positive way, this is important.


##Personal Summary

Week #2 Has been interesting and lessoning to me, “The myth of the genius programmer” hit the nail when explaining one of the most common behaviors for junior programmers which is to felt insecure or ashamed when showing your code or your work to others with more expertise, I agree with the lecture when it says that we are sabotaging ourselves from learning when we hide our work from critics or feedbacks, I think that code reviews is a very good idea too.
The videos and lectures from Linda Rising are very inspirational to me because I have been struggling with my negative mind patterns and just like her, I'm interested in how we learn and why we behavior like we do, I am older than my companions at university too so I found those lectures very motivating, I tend to jump from fixed to agile mindset from time to time and its something I actively struggle with...when I remember...so this was a nice reminder, I also found very interesting the behavioral comparison between humans and primates because I always wonder why we maintain a social structure that is not optimum in so many ways, people is really afraid to change and many won't see that we have a lot more possibilities to change our world.
I agree with the lecture called  “Programming well with others” when it states that you can create self-driven growing members or employees when you empower them and let them be responsible for their selves, although it is not an easy task because people tend to behave different at different social stimulus but it you manage your way to get the best of every situation for your team, and let them fail and learn, eventually you will get the best warriors working as a high performance team without having to be telling them to do stuff :).
The rest of the organization lectures touches good points and I definitely agree with the importance of developing assertive soft skills, it is not always easy but it is very rewarding to achieve the level of communication and respect that this skills create.
The lectures about variable length codes and data compression were very interesting, we use our computers knowing that 0's and 1's organized in bits and bytes are the foundation for many of the systems we use, but we as engineers or computer scientifics that we are (or pretend to be...) it is very important to understand this approaches and Colt McAnlis explains this concepts in such a good way, this lectures are very, very interesting, I hope some day to master this kind of manipulation over data, imagine how this concepts can be applied to Quantum computation.https://github.com/cesardariogarcia/Nearsoft-Academy-Assignments.git
