# LV-Protobuf-RAW
A low level protobuf encoder and decoder. 

This LabVIEW library allows the encoding and decoding of protobuf message buffers. 

It does NOT provide a parser or any code generation abilties needed to handle .proto definitions. But if you know what you do, you can implement messages by yourself.

A generator is worked on but is not useable by now. It will eventually be published in another project.

# Features
- Provides basic data types and conversion to / from on-wire types
  - VarINT128
    - bool
    - int32
    - int64
    - sint32
    - sint64
    - uint32
    - uint64
  - I32
    - Single
    - fixed32
    - sfixed32
  - I64
    - Double
    - fixed64
    - sfixed64
  - LEN
    - string
    - bytes
    - packed
    - message

# Usage
Build up the message hierarchy using the provided classes. 

![image](https://github.com/kleinsimon/LV-Protobuf-RAW/assets/4790227/475f9d07-c42d-4358-80b6-adbf9d1d95a0)

Use the topmost message to marshal / unmarshal the binary message data.
