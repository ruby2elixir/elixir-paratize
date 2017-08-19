Changelog
====

## Version 2.1.5 (2017-08-20)

* Bugfix: Results from `Paratize.Chunk` was overflatten, now nested list structure is preserved.
* Update docs generated from ex_doc v0.16.2.


## Version 2.1.4 (2017-01-06)

* Silence warnings for Elixir v1.4.
* Update docs generated from ex_doc v0.14.5.


## Version 2.1.3 (2016-02-23)

* Updated typespecs support for Dialyzer


## Version 2.1.2 (2016-02-14)

Bugfix & refactoring.

* Bugfix: `Paratize.TaskOptions.size` default :scheduler value was baked in
  during compile time, now determined during run time.
* Remove unnecessary Collectable protocol impl for %Paratize.TaskOptions{}.
* General refactoring


## Version 2.1.1 (2015-10-25)

* Upgrade to Elixir v1.1 as minimum supported version.
* Update docs generated from ex_doc v0.10.
* Documentation updated with CHANGELOG, README and LICENSE included.


## Version 2.1.0 (2015-08-17)

Added support for using the convenient Keyword arguments to define `%Paratize.TaskOptions`.


## Version 2.0.1 (2015-08-13)

Bugfix for tests. Improved documentation.


## Version 2.0.0 (2015-06-29)

Refactored the API again!

* Paratize.* functions are moved to their respective module.
* exec/2 are renamed to parallel_exec/2 for Paratize.Pool and Paratize.Chunk.

Common API for both `Paratize.Chunk` and `Paratize.Pool` processors.

* `parallel_exec(fun_list, task_options)`
* `parallel_map(arg_list, fun, task_options)`
* `parallel_each(arg_list, fun, task_options)`
