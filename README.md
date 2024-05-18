# osh-registry: A registry of Open Source Hardware (OSH) projects


This is a work-in-progess in early stages.

## The Idea

This repo is modeled after the [Arduino Library Registry](https://github.com/arduino/library-registry)
and the way it works. The idea is to allow new open source hardware projects to be registered
here by making a pull request against a simple flat file that adds a new project.
In this way the public is encouraged to add new projects.

    However, the Arduino community is mature and has a standardized and accepted in the libary.json
    file format. No consensus has yet formed in the open source hardware community, although
    we advocate the [Open Know-How (OKH)](https://standards.internetofproduction.org/pub/okh/release/1)
    standard.

    We are seeking a registry that can take advantage of the OKH, but does not rely on it,
    or even depend on git as a hosting mechanism.

## The osh-registry.json file Format

    The osh-registry.json file format uses JavaScript Object Notation (JSON) to define entries.
    The file itself is technically a list of JavaScript objects.

    A prototypical entry looks something like:

```
{
    "name": "VentMon",
    "projectOrRegistry": "project",
    "keywords": "spirometer, respiration, Arduino, ESP32",
    "description": "VentMon: An open source IoT-enabled spriometer for testing medical ventilators",
    "okh": "https://github.com/PubInv/ventmon-ventilator-inline-test-monitor/blob/master/ventmon-okh.yml",
    "human-url": "https://www.pubinv.org/project/ventmon/",
    "repository": {
        "type": "git",
        "url": "https://github.com/PubInv/ventmon-ventilator-inline-test-monitor"
    },
    "hardwareLicense": CERN-OHL-S",
    "authors": [
    {
      "name": "Robert L. Read",
      "email": "read.robert@gmail.com",
      "url": "https://github.com/RobertLRead",
      "maintainer": true
    },
    {
      "name": "Ben Coombs",
    },
    {
      "name": "Lauria Clarke",
    }
    ],
    "version": "0.5",
}
```

## The Live Site
When you are ready, please visit the [live website](https://pubinv.github.io/osh-registry/).
