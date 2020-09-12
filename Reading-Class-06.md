# Redis
https://aws.amazon.com/redis/

* Stands for "Remote Dictionary Server"
  * open-source data store
* data resided in-memory instead of on disks or SSDs
  * gets data faster!
* popular to use for caching, chat, game leaderboards, streaming, geospatial data, machine learning, etc

# What is a queue?
https://www.educative.io/edpresso/what-is-a-queue

* common data structure that places elements in a sequence
  * uses First in First out method

  # Task queues
  https://redislabs.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/

  * "When handling requests from web clients, sometimes operations take more time to
execute than we want to spend immediately. We can defer those operations by putting
information about our task to be performed inside a queue, which we process later.
This method of deferring work to some task processor is called a task queue. Right now
there are many different pieces of software designed specifically for task queues
(ActiveMQ, RabbitMQ, Gearman, Amazon SQS, and others), but there are also ad hoc
methods of creating task queues in situations where queues aren’t expected. If you’ve
ever had a cron job that scans a database table for accounts that have been modified/
checked before or after a specific date/time, and you perform some operation based
on the results of that query, you’ve already created a task queue."

# First in First out Queues
https://redislabs.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/6-4-1-first-in-first-out-queues/

* so basically the thing at the beginning of the queue is going to be the first thing executed and the last thing will be the last thing executed. And new things are added to the back of the queue

# Bull's Guide
https://optimalbits.github.io/bull/

* a node library that implements a fast queue system based of redis

* you create a queue by creating a bull instance
  * an instance can have 3 different roles: job producer, job consumer and event listener

* producers add jobs to the queue

* consumers are programs that define process functions

* listeners listen for events
  * can be local and only receive notifications in a given queue instance
  * or global and listen to all of the events in the queue