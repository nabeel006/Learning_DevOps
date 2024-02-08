Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content, such as .html, .css, .js, and image files, to your users. CloudFront delivers your content through a worldwide network of data centers called edge locations. When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency (time delay), so that content is delivered with the best possible performance.

SEO of your website like keywords.
Data retrieval shuld be fast


you can use it in the streaming scenario.
![[how-you-configure-cf.png]]



- Amazon CloudFront is a content delivery network (CDN) offered by AWS.
    
- CDN provides a globally-distributed network of proxy servers which cache content , i.e., web videos or other bulky media, more locally to consumers, thus improving access speed for downloading the content.
    
- CloudFront service works on a pay-as-you-go basis.
    
- CloudFront works with origin servers like S3, EC2 where the content is stored and is pushed out to multiple CloudFront servers as content is requested.
    
- When CloudFront is enabled, the content is stored on the main S3 server.
    
- Copies of this content are created on a network of servers around the world called CDN.
    
- Each server within this network is called an Edge server, which will only have a copy of your content.
    
- When a request is made to the content, the user is provided from the nearest edge server.
    
- CloudFront has features similar to dynamic site acceleration, a method used to improve online content delivery.
    
- CloudFront accelerates the delivery of dynamic content by moving it closer to the user to minimize internet hops involved in retrieving the content.
    
- CloudFront's Web distribution supports "**Progressive**" download i.e., data from S3 is cached and then streamed without disruptions.
    
- Due to that, the user cannot move front or back in the video i.e., the video is processed bit by bit.
    
- CloudFront's Web distribution support "**Streaming**" allows users to directly watch without any download.
    
- Due to that, the user can move front or back in the video, the latency is based on the size of the file and the customer's Internet bandwidth.
    
- This service is beneficial for those developing a website that distributes a lot of content and needs to scale-up.
    
- It helps reduce costs and improve the performance of a website by providing high data transfer speeds and low latency.  
     
    

# Architecture Diagram

![](https://labresources.whizlabs.com/35b5214b5298cb78a0d4e287e6698091/2._introduction_to_amazon_cloudfront_27_27.png)
## How you set up Cloud Front to deliver content
