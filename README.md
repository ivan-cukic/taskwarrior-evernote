# Evernote feeder for Taskwarrior

Pulls notes from Evernote that have specific tag and adds them
to Taskwarrior as tasks.

You need to set a few UDAs to Taskwarrior for this to work properly:

    uda.evernote_url.type=string
    uda.evernote_url.label=Evernote URL
    uda.evernote_id.type=string
    uda.evernote_id.label=Evernote ID

## Usage:

    taskwarrior-evernote-sync               Pulls the notes from Evernote
    taskwarrior-evernote-sync --list-tags   Lists Evernote tags and their UUIDs
    taskwarrior-evernote-sync --help        This message

## Configuration options:

    tag_uid        UID of the Evernote tag (required)
    project        Tasks imported from Evernote will have this project set (default='evernote')

## Requirements

 - You need to set up GeekNote[1] and Taskwarrior[2] properly
 - You need configobj, termcolor, bs4 and taskw python2 modules

