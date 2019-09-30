# mcgonagle/103

[![Docker Automated Build](https://img.shields.io/docker/automated/mcgonagle/103.svg?style=flat-square)](https://hub.docker.com/r/mcgonagle/103/) [![Apache-2.0 License](https://img.shields.io/github/license/mcgonagle/103.svg?style=flat-square)](https://github.com/mcgonagle/103/blob/master/LICENSE) [![Docker Build Status](https://img.shields.io/docker/build/mcgonagle/103.svg?style=flat-square)](https://hub.docker.com/r/mcgonagle/103/builds/)

This is a basic Docker image for building and previewing [Hovercraft](https://github.com/regebro/hovercraft) the 103 presentation. The image is available for public use on Docker Hub at [mcgonagle/103](https://hub.docker.com/r/mcgonagle/103/).

## Usage

To Build:
``` bash
docker build --tag=mcgonagle/103 .
```

To Run:
``` bash
docker run -it --rm -p "9000:9000" mcgonagle/103
```

In a web browser, go to <http://localhost:9000> to view your presentation.

