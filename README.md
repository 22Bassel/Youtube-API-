# Youtube-API-
Springboot Youtube API  (V3) app ,the app works in a deployed way with Eurka (Microservices). it has 3 main functions that access to real Youtube .the functions : add like, search ,and add comment then show all comments. Also there is getway .the "add like" works with RubbitMQ ,but other services use Restful API .and search service uses mysql DB. 

to use search service you have to get API KEY (without authentication), but in other services you have to get token from your youtube account. you can see this site :https://stevesie.com/docs/pages/youtube-oauth-access-token . 
but select the option youtube.force-ssl intsteade of youtube.readonly . 
Also add like service need RabbitMQ , the queue it uses have to call : Like_queue . 
Search service is a statefull service , it saves some data about user in DB.
