bu kod lambda yada normal servis olarak deploy edileblir. 

her iki durum icin de 2 tane aws reource una ihtiyacin var biri s3 bucket digeri sqs queue. Queue name `serverless-sqs` bucket name `bucket-picture` olacak. 
Bu iki deger kodda hardcoded olarak duruyor bunlari env ye cikarman daha mantikli olur. 

lambda yapmak istersen onune bir api-gw lazim api gateway de 2 endpoint bu lambda ya gelecek biri `/login` endpoint i digeri `/` endpoint i 
iki endpoint e de yapilan post requestleri bu lambda yi trigger edecek sekilde api gateway setup edilmeli.

login endpoint i jwt token generate ediyor bu token ile diger enpoint i cagirman lazim.

