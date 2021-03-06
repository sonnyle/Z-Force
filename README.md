> Copyright (c) 2013 Zuora, Inc.
> 
> Permission is hereby granted, free of
> charge, to any person obtaining a copy
> of  this software and associated
> documentation files (the "Software"),
> to use copy,  modify, merge, publish
> the Software and to distribute, and
> sublicense copies of  the Software,
> provided no fee is charged for the
> Software.  In addition the rights
> specified above are conditioned upon
> the following: The above copyright
> notice and this permission notice
> shall be included in all copies or
> substantial portions of the Software.
> Zuora, Inc. or any other trademarks of
> Zuora, Inc.  may not be used to
> endorse or promote products derived
> from this Software without specific
> prior written permission from Zuora,
> Inc. THE SOFTWARE IS PROVIDED "AS IS",
> WITHOUT WARRANTY OF ANY KIND, EXPRESS
> OR IMPLIED, INCLUDING BUT NOT LIMITED
> TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND
> NON-INFRINGEMENT. IN NO EVENT SHALL
> ZUORA, INC. BE LIABLE FOR ANY DIRECT,
> INDIRECT OR CONSEQUENTIAL DAMAGES
> (INCLUDING, BUT NOT LIMITED TO,
> PROCUREMENT OF SUBSTITUTE GOODS OR
> SERVICES; LOSS OF USE, DATA, OR
> PROFITS; OR BUSINESS INTERRUPTION)
> HOWEVER CAUSED AND ON ANY THEORY OF
> LIABILITY, WHETHER IN CONTRACT, STRICT
> LIABILITY, OR TORT (INCLUDING
> NEGLIGENCE OR OTHERWISE) ARISING IN
> ANY WAY OUT OF THE USE OF THIS
> SOFTWARE, EVEN IF ADVISED OF THE
> POSSIBILITY OF SUCH DAMAGE.

**Zuora for Salesforce Sample Code Suite**
--

**Introduction**
--

The Zuora for Salesforce Sample Code Suite provides executable code examples in unmanaged Force.com packages. 

Zuora Support does not troubleshoot content from GitHub. The sample code is as an example of code 
that has worked for previous implementations and was created by both Zuora and non-Zuora authors. 

**Pre-Requisites**
--

* The Zuora for Salesforce Sample Code Suite includes a set of unmanaged packages that depend on the following Z-Force managed packages:
  * Zuora for Salesforce 360 Version 2.2 or above
  * Zuora for Salesforce Quotes Version 5.3 or above

* If you do not have Force.com Migration Tool already installed and you would like to use the Force.com Migration Tool to deploy the sample code to your Salesforce.com organization, please follow the instructions below: 
  * Visit http://java.sun.com/javase/downloads/index.jsp and install Java JDK, Version 6.1 or greater on the deployment machine.
  * Visit http://ant.apache.org/ and install Apache Ant, Version 1.6 or greater on the deployment machine.
  * Set up the environment variables (such as ANT_HOME, JAVA_HOME, and PATH) as specified in the Ant Installation Guide at http://ant.apache.org/manual/install.html.
  * Log in to Salesforce on your deployment machine. Click Your Name | Setup | Develop | Tools, then click Force.com Migration Tool.
  * Unzip the downloaded file to the directory of your choice. The Zip file contains a Jar file containing the ant tasks: ant-salesforce.jar
  * Copy the ant-salesforce.jar file from the unzipped file into the ant lib directly.  The ant lib directly is located in the root folder of your Ant installation. 

**Installation Instructions**
--

* Open ZForce/build.properties, and specify the login credentials for your Salesforce.com organization: 

    >sf.username=
    
    >sf.password= 

Please note that the password should be your login password concatenated with the security token.

* Navigate to Z-Force folder, and type the following in the command line: 

    >ant deploy

This will deploy all sample code packages to your Salesforce.com organization.

Optionally, you can deploy one or more sample code packages individually into one or more Salesforce.com organizations. 
  * Navigate to Z-Force/<Sample Code Package> folder, for instance, Z-Force/InvoiceOwnerTransfer
  * Open build.properties file, and specify the login credentials for your Salesforce.com organization (for this specific sample code package)

    >sf.username=    
    >sf.password= 
    
* In command-line, type:

    >ant deploy

This will deploy the specific sample code package into your Salesforce.com organization.
