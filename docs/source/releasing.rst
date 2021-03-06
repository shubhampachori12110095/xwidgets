.. Copyright (c) 2017, Johan Mabille and Sylvain Corlay

   Distributed under the terms of the BSD 3-Clause License.

   The full license is in the file LICENSE, distributed with this software.

Releasing xwidgets
==================

Releasing a new version
-----------------------

From the master branch of xwidgets

- Make sure that you are in sync with the master branch of the upstream remote.
- In file ``xwidgets_config.hpp``, set the macros for ``XWIDGETS_VERSION_MAJOR``, ``XWIDGETS_VERSION_MINOR`` and ``XWIDGETS_VERSION_PATCH`` to the desired values.
- Update the README file w.r.t. dependencies on xwidgets.
- Update the environment.yml file used by binder with the new version of
  xwidgets and dependencies.
- Stage the changes (``git add``), commit the changes (``git commit``) and add a tag of the form ``Major.minor.patch``. It is important to not add any other content to the tag name.
- Push the new commit and tag to the main repository. (``git push``, and ``git push --tags``)
- Release xwidgets on conda.
- Change the binder link in the REAME and commit this change.
