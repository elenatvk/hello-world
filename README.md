# hello-world
My first github project!
* This line is new
** And this
* And this
*** Hmm what does this do?
// And this?

# What about this one?

## New topic?

 | One     | Two        | Three   | Four          | 
| ------------- |-------------| ---------| ------------- |
| One                | Two               | Three          | Four                |

| One     | Two        | Three   | Four          | 
| ------------- |-------------| ---------| ------------- |
| Span Across ||||

<table>
  <tr>
    <td>One</td>
    <td>Two</td>
  </tr>
  <tr>
    <td colspan="2">Three</td>
  </tr>
</table>

The following table lists the sample infrastructure micro templates	and describes what they provision.

Template Folder on GitHub| Provisions Platform Manager
-------------------------|--------------------------------
[sag-spm-boot-local](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-boot-local) | on the same host as Command Central
[sag-spm-boot-ssh](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-boot-ssh) | on remote UNIX hosts using SSH protocol
[sag-spm-boot-winrm](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-boot-winrm) | on remote Windows hosts using the native	Windows remote protocol, which eliminates the requirement for SSH access
[sag-spm-connect](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-connect) | connects to existing Platform Manager nodes

### Run-time Micro Templates

The following table lists the sample run-time micro templates for each Software AG product and describe what they provision.

<table>
  <tr>
    <th>Software AG Product</th>
    <th>Template Folder onGitHub</th>
    <th>Provisions</th>
  </tr>
  <tr>
    <td>Asset Build Environment</td>
    <td>[sag-abe](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-abe)</td>
    <td>webMethods Asset Build Environment</td>
  </tr>
  <tr>
    <td>Apama</td>
    <td>[sag-apama-correlator](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-apama-correlator)</td>
    <td>Apama correlator instance</td>
  </tr>
  <tr>
    <td>Designer</td>
    <td>[sag-designer-services](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-designer-services)</td>
    <td>Service Development</td>
  </tr>
  <tr>
    <td>EntireX</td>
    <td>[sag-exx-broker](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-exx-broker)</td>
    <td>webMethods EntireX</td>
  </tr>
  <tr>
    <td rowspan="5">Integration Server</td>
    <td>[sag-is-applatform](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-is-applatform)</td>
    <td>webMethods Integration Server with webMethods Application Platform</td>
  </tr>
  <tr>
    <td>[sag-is-cluster](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-is-cluster)</td>
    <td>a stateless Integration Server cluster</td>
  </tr>
  <tr>
    <td>[sag-is-server](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-is-server)</td>
    <td>a core Integration Server installation</td>
  </tr>
  <tr>
    <td>[sag-is-statefull-cluster](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-is-statefull-cluster)</td>
    <td>an Integration Server installation cluster with Terracotta BigMemory</td>
  </tr>
  <tr>
    <td>[sag-msc-server](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-msc-server)</td>
    <td>webMethods Microservices Runtime instance</td>
  </tr>
  <tr>
    <td rowspan="3">Terracotta</td>
    <td>[sag-tc-cluster](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-tc-cluster)</td>
    <td>a Terracotta BigMemory cluster with two nodes</td>
  </tr>
  <tr>
    <td>[sag-tc-server](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-tc-server)</td>
    <td>a Terracotta BigMemory server</td>
  </tr>
  <tr>
    <td>[sag-tdb-server](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-tdb-server)</td>
    <td>a Terracotta DB server</td>
  </tr>
  <tr>
    <td rowspan="2">Universal Messaging</td>
    <td>[sag-um-cluster](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-um-cluster)</td>
    <td>Software AG Universal Messaging cluster with two nodes</td>
  </tr>
  <tr>
    <td>[sag-um-server](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-um-server)</td>
    <td>Universal Messaging realm server</td>
  </tr>
</table>

### Micro Templates for Configuring Command Central and Platform Manager

The following table lists the sample run-time micro templates for configuring Command Central and Platform Manager and describes what they do.

Template Folder on GitHub| Provisions Platform Manager
-------------------------|--------------------------------
[sag-cc-builder-dev](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-builder-dev) | Creates product, fix, and asset repositories.
[sag-cc-creds-dev](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-creds-dev) | Configures different types of credentials for accessing repositories and remote hosts, including basic username/password	authentication, SSH private key authentication, and authentication with	encrypted passwords.
[sag-cc-creds](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-creds) | Configures default outbound credentials for Command Central.
[sag-cc-layer-defs](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-layer-defs) | Creates Software AG base layer type definitions.
[sag-cc-ldap](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-boot-local) | Creates a sample Command Central configuration for LDAP containing users, groups and roles.
[sag-cc-mirrors](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-mirrors) | Registers to remote mirrors using default credentials.
[sag-cc-repos-asset](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-repos-asset) | Creates a sample asset repository.
[sag-cc-tuneup](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-cc-tuneup) | Configures Command Central and Platform Manager for tuning and troubleshooting.
[sag-db-oracle](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-db-oracle) | Creates a user, database, and webMethods database schemas on an Oracle database server.
[sag-spm-config](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-config) | Configures Platform Manager.
[sag-spm-proxy](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-spm-proxy) | Creates a proxy configuration for Platform Manager.
[sag-update](https://github.com/SoftwareAG/sagdevops-templates/tree/master/templates/sag-update) | Installs the latest fixes from Empower.
