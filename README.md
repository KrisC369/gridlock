# GridLock

GridLock is a Java based microscopic traffic simulator aimed at evaluation distributed traffic coordination systems.  It is developed to evaluate ongoing research in traffic coordination by the AgentWise group at the DistriNet Labs of the Univerity of Leuven, Belgium.

## Cloning instructions

GridLock is divided in several modules.  The module structure is represented both in the Maven project structure and the git repository structure.  Submodules are configured as Maven submodules and each submodule has its own git repository and is included in the parent project as a git submodule.  To get a complete and working copy of the code you have to clone the master `gridlock` project, update the submodules and build the maven project.

    git clone git://github.com/rutgerclaes/gridlock.git
    cd gridlock
    git submodule init
    git submodule update
    mvn validate
    mvn install
