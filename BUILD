# Copyright 2020 Pants project contributors.
# Licensed under the Apache License, Version 2.0 (see LICENSE).

# A macro that turns every entry in this directory's requirements.txt into a
# `python_requirement_library` target. Refer to
# https://www.pantsbuild.org/docs/python-third-party-dependencies.
python_requirements(name="reqs", resolve="python-default")
python_requirements(name="other-reqs", resolve="python-other")

__defaults__(all=dict(resolve=parametrize("python-default", "python-other")))

