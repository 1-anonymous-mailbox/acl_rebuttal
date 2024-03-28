## Example 1

**persona descriptions:** 

(1) i read twenty books a year. 

(2) i am a stunt double as my second job. 

(3) i only eat kosher. 

(4) i was raised in a single parent household.

**dialogue history:**

hello what are doing today?

| Model  | generated candidate responses                                |
| ------ | ------------------------------------------------------------ |
| BART   | hi, i am doing well. how are you?<br/>hi, i am doing well. how about you?<br/>hi, i am just reading a book. you? <br/>(The candidate responses are highly similar and only use one sentence of persona description, "I read twenty books a year.")|
| Llama2 | i am reading a book, i read 20 books a year. what are you doing?<br/>i am reading a book. i read 20 books a year. what are you doing?<br/>i am reading, i love to read! how about you? <br/>(only considered one persona description "I read twenty books a year.")|
| LMEDR  | i am reading a book. how about you?<br/>i am reading a book. i read about 20 a year. how about you?<br/>i am reading a book. how about you?  <br/>(The candidate responses are highly similar and only use one sentence of persona description, "I read twenty books a year.")|
| KPDD   | i am reading a book. how are you doing? any plans for the weekend?<br/>i just got off work. a little tired. how are you?<br/>i am good thanks for asking. how are you? i am a stunt double. what about you?<br/>(The candidate responses exhibit high diversity, and multiple persona descriptions are considered, including "I read twenty books a year" and "I am a stunt double as my second job.")|



## example 2

**persona descriptions:** 

(1) i read twenty books a year. 

(2) i am a stunt double as my second job. 

(3) i only eat kosher. 

(4) i was raised in a single parent household.

**dialogue history:**

user: hello what are doing today?

model: i am good , i just got off work and tired , i have two jobs .

user: i just got done watching a horror movie

| Model  | generated candidate responses                                |
| ------ | ------------------------------------------------------------ |
| BART   | i am a stunt double for a living, i love horror movies.<br/>i am a stunt double for a living.<br/>i am a stunt double, i do not like horror movies. |
| Llama2 | i do not watch those, too scary. what do you do for a living?<br/>i do not watch horror movies, i am a jewish and do not believe in it .<br/>oh wow, i do not like horror movies. |
| LMEDR  | i have a second job as a stunt double.<br/>i just got off work as well. i'm a stunt double for a movie.<br/>i work as a stunt double for a movie company. |
| KPDD   | It sounds scary. i do stunts for a living, what are you doing?<br/>i love horror movies! i am a stunt double, i do double duty as well.<br/>what is it called?  is it good or bad? |
