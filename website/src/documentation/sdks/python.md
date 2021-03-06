---
layout: section
title: "Apache Beam Python SDK"
section_menu: section-menu/sdks.html
permalink: /documentation/sdks/python/
---
<!--
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->
# Apache Beam Python SDK

The Python SDK for Apache Beam provides a simple, powerful API for building batch and streaming data processing pipelines.

## Get started with the Python SDK

Get started with the [Beam Python SDK quickstart]({{ site.baseurl }}/get-started/quickstart-py) to set up your Python development environment, get the Beam SDK for Python, and run an example pipeline. Then, read through the [Beam programming guide]({{ site.baseurl }}/documentation/programming-guide) to learn the basic concepts that apply to all SDKs in Beam.

See the [Python API reference](https://beam.apache.org/releases/pydoc/) for more information on individual APIs.

## Python streaming pipelines

Python [streaming pipeline execution]({{ site.baseurl }}/documentation/sdks/python-streaming)
is experimentally available (with some [limitations]({{ site.baseurl }}/documentation/sdks/python-streaming/#unsupported-features))
starting with Beam SDK version 2.5.0.

## Python type safety

Python is a dynamically-typed language with no static type checking. The Beam SDK for Python uses type hints during pipeline construction and runtime to try to emulate the correctness guarantees achieved by true static typing. [Ensuring Python Type Safety]({{ site.baseurl }}/documentation/sdks/python-type-safety) walks through how to use type hints, which help you to catch potential bugs up front with the [Direct Runner]({{ site.baseurl }}/documentation/runners/direct/).

## Managing Python pipeline dependencies

When you run your pipeline locally, the packages that your pipeline depends on are available because they are installed on your local machine. However, when you want to run your pipeline remotely, you must make sure these dependencies are available on the remote machines. [Managing Python Pipeline Dependencies]({{ site.baseurl }}/documentation/sdks/python-pipeline-dependencies) shows you how to make your dependencies available to the remote workers.

## Creating new sources and Sinks

The Beam SDK for Python provides an extensible API that you can use to create new data sources and sinks. [Creating New Sources and Sinks with the Python SDK]({{ site.baseurl }}/documentation/sdks/python-custom-io) shows how to create new sources and sinks using [Beam's Source and Sink API](https://github.com/apache/beam/blob/master/sdks/python/apache_beam/io/iobase.py).
