---
title: Python Examples
menu: Examples 
weight: 20
---

{{< caution >}}

Only producers and consumers are supported. There is no support for cluster administration.

Also client does not support [async python](https://docs.python.org/3/library/asyncio.html).

{{</ caution >}}

* The Python client [wraps the rust client](https://www.infinyon.com/blog/2021/03/python-client/).
* It currently does not support the administrator features that the rust client does.
* The [PartitionConsumer.stream](https://infinyon.github.io/fluvio-client-python/fluvio.html#PartitionConsumer.stream) returns an object which implements the [python iterator convention](https://wiki.python.org/moin/Iterator) to allow for iterating over the stream in a for-loop.

To see the full docs, visit our [pdoc page](https://infinyon.github.io/fluvio-client-python/fluvio.html).
## Example Workflow

Follow the [installation instructions]({{< ref "installation.md" >}}) to run this example.

{{<code file="embeds/client-examples/python/hello-python.py" lang="python" copy=true >}}

### Run

%copy first-line%
```shell
$ python hello-python.py
```

## Links to Docs:
* [Connect to Fluvio](https://infinyon.github.io/fluvio-client-python/fluvio.html#Fluvio.connect)
* [Get a Producer](https://infinyon.github.io/fluvio-client-python/fluvio.html#Fluvio.topic_producer)
* [Send to Topic](https://infinyon.github.io/fluvio-client-python/fluvio.html#TopicProducer.send)
* [Get a Consumer](https://infinyon.github.io/fluvio-client-python/fluvio.html#Fluvio.partition_consumer)
* [Get a Stream](https://infinyon.github.io/fluvio-client-python/fluvio.html#PartitionConsumer.stream)
