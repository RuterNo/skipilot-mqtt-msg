# Skipilot MQTT Messages

## Overview

This API describes a set of MQTT topics which are used to distribute information about vehicle schedule,vehicle activity, vehicle status and bookings between Konsentra/Trapeze, Ruter and Holo/Sensible 4.

## Consumer Client Requirements

Consumers should be aware of and handle:
- Optional properties that can be null or left out
- Arrays can contain any number of elements including zero

## Quality of Service and different flags
Use QoS level 2 for topics

Set retain flag to false for most of the topics

Subscibers should start with clean session set to true.

All data must be JSON and UTF-8 encoded. Topics are categorized by a thematic perspective, according to the topic structure proposed for ITxPT at the time of writing.

## Topic names

Topic names are generally written on the format of {recipient}/{sender}/{vehicleid}/{topic} to make it easy to identify the source and destination of the messages. 

# Versions

Version                                | datetime                                                              | changes      |
| :---------------------------------- | :----------------------------------------------------------------------- |--------------|
[v2.0](v2.0/README.md) | 2021-08-19 11:00 | Second draft |
[v1.0](v1.0/README.md) | 2021-05-25 14:00 | First draft  |
 
# Abbreviations

Keyword                                | Desc                                      |
| :---------------------------------- |:------------------------------------------|
av | Autonomous Vehicle                        |
vin | Vehicle Identification Number (vehicleId) |
vaid | Vehicle Activity ID                       |
--- 

