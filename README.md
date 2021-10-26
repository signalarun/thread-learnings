# Thread-learnings
Information on threads


## Java Snipets
1. ``` Runtime.getRuntime().availableProcessors(); ```
2. Cached thread pool
   These are used for IO intensive operations
   ```
     Runnable job = () -> {
       try{
         Thread.sleep(20);
       }catch(InterruptedException e){
         System.println(e.printStackTrace());
       }
       Sysem.out.println(Thread.currentThread().getName());
     }
     
     ExecutorService executor = Executors.newCachedThreadPool(); // creating cached threadpool
     
     for(int i=0; i<10; i++){
      executor.execute(job); // executing the job with cached threadpool
     }
     
   ```
4. 

## Tutorials
 1. [![](https://res.cloudinary.com/marcomontalbano/image/upload/v1630489099/video_to_markdown/images/youtube--6Oo-9Can3H8-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=6Oo-9Can3H8 "")
 2. [![Executor Service - Pool Types](https://res.cloudinary.com/marcomontalbano/image/upload/v1630495264/video_to_markdown/images/youtube--sIkG0X4fqs4-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=sIkG0X4fqs4 "Executor Service - Pool Types")
 3. [![Completable Future](https://res.cloudinary.com/marcomontalbano/image/upload/v1634889451/video_to_markdown/images/youtube--ImtZgX1nmr8-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=ImtZgX1nmr8 "Completable Future")
 4. [![Ideal threadpool size](https://res.cloudinary.com/marcomontalbano/image/upload/v1635137868/video_to_markdown/images/youtube--ErNre5varF8-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=ErNre5varF8 "Ideal threadpool size")
 5. https://mkyong.com/java/java-scheduledexecutorservice-examples/
