Change Log For PyCliProg
========================


PyCliProg 0.2.0 - 2017-XX-XX
----------------------------

- Removed names

  - throwing ``ArgumentParser`` & ``ArgError``
  - ``Prog.add_basic_args``

    Merged into ``Prog.add_logging_args``

- Added names

  - A logger is available via ``self.logger``

- Added shorthands

  - ``Prog.add_arg``

- Other Changes

  - Removed the short option ``-L``, the long option unchanged
  - Removed the short option ``-A``, the long option unchanged
  - Fixed ``--append-log`` to be a ``store_true`` action
  - Grouped the options ``-v/--verbose`` and ``-q/--quiet`` into ``Logging Levels``, ``--log-file`` and ``--append-log`` into ``Logging Files``


PyCliProg 0.1.0 - 2017-03-30
----------------------------

``0.1.0`` is the first public pre-release.

- Added names that are considered public

  - the ``Prog`` class
  - the ``ExitFailure`` exception class

  You won't be prevented from importing any other names,
  but the aforementioned two are the most useful ones.

- Methods that are considered public and should be overridden

  - ``Prog.main``
  - ``Prog.add_args``

  Other methods are considered advanced,
  but not reserved nor internal.
