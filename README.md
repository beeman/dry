# Don't Repeat Yourself

Code generation for XPages


## Commands

### Creating a new project

    $ dry create-project <NewProject>
      - dry creates directories for NewProject
      - dry creates project files



## Command line parameters

    Command         Alias  Description
    create-project  cp     Initialize new project structure

## Project Skeleton

### Initial directory structure

    AppProperties
    Code
    CustomControls
    Forms
    Resources
    Views
    WebContent
    WebContent/WEB-INF
    XPages

### Files

#### .classpath
    <?xml version="1.0" encoding="UTF-8"?>
    <classpath>
      <classpathentry kind="src" path="Local"/>
      <classpathentry kind="con" path="org.eclipse.jdt.launching.JRE_CONTAINER"/>
      <classpathentry kind="con" path="org.eclipse.pde.core.requiredPlugins"/>
      <classpathentry kind="output" path="WebContent/WEB-INF/classes"/>
    </classpath>

#### .project
    <?xml version="1.0" encoding="UTF-8"?>
    <projectDescription>
    	<name>******PROJECT_NAME******</name>
    	<comment></comment>
    	<projects>
    	</projects>
    	<buildSpec>
    		<buildCommand>
    			<name>com.ibm.designer.domino.team.builder.PhysicalToNsfSynBuilder</name>
    			<arguments>
    			</arguments>
    		</buildCommand>
    	</buildSpec>
    	<natures>
    	</natures>
    </projectDescription>


## Extra possible functionality:

* Automatically initialize / commit git repo
* Automatically add README.md
* Automatically add LICENSE (user input on which license)
