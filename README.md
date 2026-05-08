This is a repo containing the results of participating in a lab to create an article-writing agent
The Lab is hosted by Kirill Eremenko and it is recorded at this URL: https://www.loom.com/share/81c3117188ad4392af59e2189168d479

The lab is suposed to implement:
- a search web tool that looks for web pages related to the input topic
- a fetch URL tool that downloads the contents of URLs
- a research agent that uses the search web tool and fetch URL tool to get content from the web and write a research brief with the downloaded content
- a writer agent that uses a research brief to write a professional article
- an orchestrator agent that receives the topic to investigate and uses the research agent to produce two research briefs, then choose the best of them and use the writer agent to produce an article about the topic.
- input guardrail that will filter the user input topic and block the process if it is one of the forbidden topics
- output guardrail (not yet working) that will filter the produced article and dismiss it if it contains one of the forbidden topics

The output guardrail was suposed to be "homework". The whole got to the point where everything worked except for the output guardrail, not yet implemented at the time.
Then I disabled the input guardrail, so it would let pass forbidden topics and tried to implement the output guardrail. But it is never called. Articles about the forbidden topics are produced without error.
