### Version 1.5 (April 2, 2014)

* Support for starting and stopping containers with the help of Cargo daemon.

### Version 1.4.1 (March 22, 2014)

* `cargoStartLocal` and `cargoRunLocal` fail if log file doesn't exist - [Issue 83](https://github.com/bmuschko/gradle-cargo-plugin/issues/83).
* Renamed property `output` to `outputFile`.
* Some of the input properties needed to be `Serializable`.

### Version 1.4 (February 15, 2014)

* Added sharedClasspath and extraClasspath support for local containers - [Pull request 73](https://github.com/bmuschko/gradle-cargo-plugin/pull/77).

### Version 1.3 (January 25, 2014)

* Broke out base plugin to allow full control for creating and configuring deployment tasks.
* The Cargo libraries now get pre-configured. A custom Cargo version can still be assigned via the configuration `cargo`.

### Version 1.2.2 (January 06, 2013)

* Fix input annotation for `configHomeDir` property - [Pull request 73](https://github.com/bmuschko/gradle-cargo-plugin/pull/73).

### Version 1.2.1 (December 28, 2013)

* Fixed missing property `UNDEPLOY_ACTION` on remote task - [Issue 72](https://github.com/bmuschko/gradle-cargo-plugin/issues/72).

### Version 1.2 (December 24, 2013)

* Create custom task types for each action - [Issue 20](https://github.com/bmuschko/gradle-cargo-plugin/issues/20).

### Version 1.1 (December 16, 2013)

* Adding support of the cargo timeout property - [Pull request 66](https://github.com/bmuschko/gradle-cargo-plugin/pull/66).
* Harden validation code for deployables - [Issue 67](https://github.com/bmuschko/gradle-cargo-plugin/issues/67).
* Add support for passing system properties to container - [Issue 68](https://github.com/bmuschko/gradle-cargo-plugin/issues/68).

### Version 1.0 (December 15, 2013)

* Allow configuring container using generic properties.
* Update of supported containers.
* Upgrade to Gradle Wrapper 1.9.

### Version 0.6.1 (July 21, 2013)

* Support for Jetty 9.x - [Pull request 48](https://github.com/bmuschko/gradle-cargo-plugin/pull/48).
* Fix deprecation warnings in gradle 1.6 - [Pull request 48](https://github.com/bmuschko/gradle-cargo-plugin/pull/42).
* Adding support for specifying configuration home - [Pull request 40](https://github.com/bmuschko/gradle-cargo-plugin/pull/40).

### Version 0.6 (April 16, 2013)

* Avoid having to assign the WAR file for a remote undeploy action - [Issue 30](https://github.com/bmuschko/gradle-cargo-plugin/issues/30).
* _Note:_ This release requires you to use Cargo >= 1.3.3.

### Version 0.5.9 (March 8, 2013)

* Added configuration option for binary files - [Pull request 33](https://github.com/bmuschko/gradle-cargo-plugin/pull/32).

### Version 0.5.8 (February 25, 2013)

* Capturing Cargo Ant logging - [Pull request 33](https://github.com/bmuschko/gradle-cargo-plugin/pull/33).
* Upgrade to Gradle Wrapper 1.4.

### Version 0.5.7 (January 13, 2013)

* Avoid masking exceptions thrown in build.gradle - [Issue 29](https://github.com/bmuschko/gradle-cargo-plugin/issues/29).
* Some of the container-specific task property classes did not implement TaskProperty - [Issue 27](https://github.com/bmuschko/gradle-cargo-plugin/issues/27).

### Version 0.5.6 (October 14, 2012)

* Expose convention property for setting the RMI port - [Issue 21](https://github.com/bmuschko/gradle-cargo-plugin/issues/21).

### Version 0.5.5 (August 4, 2012)

* Provides support for configuration files - [Issue 14](https://github.com/bmuschko/gradle-cargo-plugin/issues/14).

### Version 0.5.4 (July 8, 2012)

* The ZIP URL installer convention property wasn't set correctly for the default local container implementation.
* Checking if all properties are set for the ZIP URL installer closure before applying it.
* Refactored duplicated code for setting the convention properties of a local container.

### Version 0.5.3 (July 7, 2012)

* Support for ZIP artifact installer - [Issue 15](https://github.com/bmuschko/gradle-cargo-plugin/issues/15).
* Upgrade to Gradle Wrapper 1.0.
* Use Groovy @Slf4j annotation for logging.

### Version 0.5.2 (December 5, 2011)

* Fixed minor bug in documentation and code about setting local container-specific properties.

### Version 0.5.1 (December 3, 2011)

* Provide convention properties for Cargo and container log files.

### Version 0.5 (November 27, 2011)

* Allow deployment of multiple artifacts - [Issue 9](https://github.com/bmuschko/gradle-cargo-plugin/issues/9). _Note:_ This slightly
changes the structure of the convention properties. Please check the documentation!

### Version 0.4 (November 27, 2011)

* Support for JVM arguments in local containers.
* Support for configuration properties specific to local container product.
* The deployable artifact can either be a WAR or an EAR file. _Note:_ This release requires your project to run with Gradle >= [1.0-m4](http://wiki.gradle.org/display/GRADLE/Gradle+1.0-milestone-4+Release+Notes).
* Upgrade to Gradle Wrapper 1.0-m6.

### Version 0.3 (June 26, 2011)

* Exposed local run task introduced in Cargo 1.1.1. The plugin does not favor the [deprecation](http://cargo.codehaus.org/Ant+support)
of the `wait` convention property. It got removed completely. Please use `cargoRunLocal` or `cargoStartLocal` depending on
your use case.
* _Note:_ This release requires you to use Cargo >= 1.1.1.

### Version 0.2 (May 30, 2011)

* Added property for setting `cargo.protocol` to remote container tasks.

### Version 0.1 (May 27, 2011)

* Initial release.