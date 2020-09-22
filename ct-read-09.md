- Redis, which stands for Remote Dictionary Server, is a fast, open-source, in-memory key-value data store for use as a database, cache, message broker, and queue.
- All Redis data resides in-memory, in contrast to databases that store data on disk or SSDs.
- A queue is another common data structure that places elements in a sequence, similar to a stack.
- A queue uses the FIFO method (First In First Out), by which the first element that is enqueued will be the first one to be dequeued.
- Enqueue() — Inserts an element to the end of the queue
- Dequeue() — Removes an element from the start of the queue
- isEmpty() — Returns true if queue is empty
- Top() — Returns the first element of the queue
- Bull is a Node library that implements a fast and robust queue system based on redis.
const myFirstQueue = new Bull('my-first-queue');
const job = await myFirstQueue.add({
  foo: 'bar'
});