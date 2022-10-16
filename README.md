# RecursiveSummarizer

GPT-3 model can generate great abstractive summarization..but suffers from a drawback ie can take only limited amount of text at a time and when it comes to its practical implementation which involves summarizing huge content of text GPT-3 cannot generate a summarization in a single take.
hence the above code contains an algoritham which first devides text into chunks of which individual summarization in generated..this individual summarization is then concatenated as a single summary and input to GPT-3.if the concatenated summary surpasses the max lenght threshold it is chunked.
this proccess is continued till the final summary lenght is close to user specified lenght intended for the final summary.

GPT-3 ada variant is used here which is fastest model but suffers a small perfomance drop compared to davinci variant...
speed is preffered here over perfomance here as lot of itterations can be expected in a summarization and a single iteration itself takes good amount of time. 
