Contributing to Perl5-Alien
=====================

Perl5-Alien is a development organization devoted to the continued development of Alien::Base and the Perl 5 Alien ecosystem as a whole.
It consists of a pumkin-holder (identified by membership in the Pumpkin team in the GitHub organization), currently Joel Berger, and the core developer team (identified by membership in the Owner team in the GitHub organization), currently they are

* Chris Marshall (chm)
* Brian Wightman (MidLifeXis)

The rules of the organization are as follows:

* The addition and modification of features is decided by majority vote or the pumpkin-holder.
* Any core developer may nominate a new one, who must then be accepted by a 2/3 majority vote.
* The pumpkin-holder has veto rights and may select their successor.
* A feature is only needed when the majority of the user base benefits from it.
* Features may only be changed or removed in a major release.  Features may be added in a minor-release.
* Refactoring and deprecations should be avoided if no important feature depends on it.
* New features can be marked as experimental to be excluded from deprecation policies.
* Only add dependencies if absolutely necessary and make them optional if possible.
* The master source code repository should always be kept in a stable state, use feature branches for actual development.
* All code contributions from non-core members should be sent as GitHub pull requests.
* No Elitism.
* Peace!

The release and version strategy is as follows:
* An official release is done by the pumpkin when a set of feature branches are merged back on to the master branch.
* A developer release may be done prior to an official release to emable CPAN tester smoking.
* The version number will follow a X.Y.Z_TAG format, where X is the major version, Y is the minor version, Z is the bugfix version number, and TAG is a token selected by the pumpkin-holder.  Z and TAG are optional in the version string.
* A major release is signaled by a new major version number.  A major release is defined as a release that changes the API in a backward-incompatible way.
* A minor relase is signaled by a new minor version number.  A minor release is defined as a release that changes the API in a backward-compatible way.
* A bugfix release is signaled by a new bugfix version number.  A bugfix release is defined as a release that does not change the API.
* If a set of features are combined into a single release, the change in the version string will change the left-most applicable part of the version string.


Alien::Base, if successful, can be a cornerstone project for other major projects.
Therefore extra care should be made to provide stability and longevity.
The project should target at least the versions of Perl that are currently supported by p5p and every attempt should be made to support older Perls if possible.
It must support Linux, Mac, and Windows.
It should attempt to support all other platforms that Perl is known to run on, where this is possible without compromising support for the major platforms listed above.

Due to the mechanisms used for automated testing, especially by CPAN Testers, and due to the nature of this, automated testing of Alien::Base is difficult.
That said, testing is of paramount importance, and every attempt should be made to have meaninful testing of Alien::Base itself as well as provide testing tools for dependent modules if possible.

(borrowed in large part from the Mojolicious project)
