### Slack API

Author: Weihan Li

Usage: slack.simple.message
       slack.link.message
       slack.detailed.message


Simple Message: slack.simple.message(text,channel)
                e.g: slack.simple.message("text","@colin")
                     slack.simple.message("text","#general")

Message with link: slack.link.message(urlText,url,text,target)
                e.g: slack.link.message("text","www.google.com","@colin","www.google.com")

Detailed Message : slack.detailed.message(target,pretext,title,title.link,text,subtitle,subcontent,imageurl,footer,footericon,color,author)
 e.g:
 slack.detailed.message(target="@colin",pretext = "pretext is here",
                         title = "title is here",title.link = "www.google.com",
                         text = "text is here",
                         subtitle = "subtitle is here"
                         subcontent="subcontnet", author = "colin",
                         imageurl = "https://platform.slack-edge.com/img/default_application_icon.png",
                         )

Upload File: slack.upload(filename,title,comments,channels)
             e.g: slack.upload("C:\\Users\\xxx\\Desktop\\combine_1.PNG",
                                "title","comments","@colin")



 Most argument are self explanatory
 @param: target which channel to post the message to (chr)
 @imageurl: put the url of a image here (chr)
