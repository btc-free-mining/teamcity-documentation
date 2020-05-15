[//]: # (title: Build Step Conditions)
[//]: # (auxiliary-id: Build Step Conditions)

When configuring a build step, you can choose a general [execution policy](configuring-build-steps.md#Execution+policy) and, since TeamCity 2020.1, add a parameter-based _execution condition_.

Execution conditions make builds more flexible and address many common use cases, such as:
* running the step only in the default branch
* running the step only in the `release` branch
* skipping the step in [personal builds](personal-build.md)

This three cases are instantly available in the build step __Add condition__ menu:

<img src="execution-conditions.png" alt="Build step execution condition"/>

Alternatively, you can select the __Other condition__ option to add the _parameter-based execution condition_, which is a logical condition that takes on input any [build parameter](configuring-build-parameters.md) provided by the TeamCity server or agent.

A build step will be executed only if all its execution conditions are satisfied in the current build run.