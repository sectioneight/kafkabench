kafkabench
##########

Just playing around with some performance numbers.

Requirements
------------

`Kafka 0.8 <http://kafka.apache.org/documentation.html#quickstart>`_ must be up
and running.

.. code-block:: bash

    $ bin/kafka-create-topic.sh --zookeeper localhost:2181 --replica 1 --partition 1 --topic benchmark
    $ go get gopkg.in/Shopify/sarama.v1

Running
-------

.. code-block:: bash

    $ go run kafkabench.go
