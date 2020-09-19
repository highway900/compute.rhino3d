# Rhino Compute Server

[![Build status](https://ci.appveyor.com/api/projects/status/unmnwi57we5nvnfi/branch/master?svg=true)](https://ci.appveyor.com/project/mcneel/compute-rhino3d/branch/master)
[![Discourse users](https://img.shields.io/discourse/https/discourse.mcneel.com/users.svg)](https://discourse.mcneel.com/c/serengeti/compute-rhino3d)

![https://www.rhino3d.com/compute](https://www.rhino3d.com/en/7.420921340460724505/images/rhino-compute-new.svg)

## REST API for RhinoCommon and Grasshopper

For more information, see https://www.rhino3d.com/compute

Compute is built on top of Rhino 7 for Windows and can run anywhere Rhino 7 for Windows can run. The two typical scenarios are:
- Running as a web server on the internet
- Running locally on a user's computer for debugging purposes

Start with the [installation guide](docs/installation.md) to setup your own Compute server, or [compile Compute](docs/installation.md#building-from-source-and-debugging) for local debugging or developing your own features.

```
iwr -useb https://raw.githubusercontent.com/mcneel/compute.rhino3d/master/script/bootstrap-server.ps1 -outfile bootstrap.ps1; .\bootstrap.ps1
```

Arguments

* `-EmailAddress EMAIL` - the Rhino download link requires a valid email
* `-ApiKey KEY` - set an API key to secure the server
* `-install` - (optional) install the compute.geometry service