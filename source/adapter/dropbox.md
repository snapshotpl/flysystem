---
layout: layout
title: Dropbox Adapter
---

# Dropbox Adapter

~~~.language-php
use Dropbox\Client;
use League\Flysystem\Filesystem;
use League\Flysystem\Adapter\Dropbox as Adapter;

$client = new Client($token, $appName);
$filesystem = new Filesystem(new Adapter($client, 'optional/path/prefix'));
~~~