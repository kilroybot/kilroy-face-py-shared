# kilroy-face-py-shared

shared code for kilroy face SDKs in Python 🤝

## Overview

This package contains code shared by SDKs related to faces.
Mostly it's just a bunch of utilities and dataclasses.

## Installing

Using `pip`:

```sh
pip install kilroy-face-py-shared
```

## Messages

Messages are dataclasses that are used in the APIs.
They are automatically generated from the protobuf definitions.

## Posts

Posts are `pydantic` models that are used to represent various types of posts.
There are definitions for:

- `TextOnlyPost`
- `ImageOnlyPost`
- `TextAndImagePost`
- `TextOrImagePost`
- `TextWithOptionalImagePost`
- `ImageWithOptionalTextPost`

## Models

One useful thing this package provides is a `SerializableModel` class.
It's a base class for `pydantic` models
that can be serialized to and from JSON
with a proper case convention.
