Welcome to a Barclamp for the Crowbar Framework project
=======================================================

The code and documentation is distributed under the [Apache 2 license](http://www.apache.org/licenses/LICENSE-2.0.html).
Contributions back to the source are encouraged.

The [Crowbar Framework](https://github.com/crowbar/crowbar) was developed by the
[Dell CloudEdge Solutions Team](http://dell.com/openstack) as a [OpenStack](http://OpenStack.org) installer but has
evolved as a much broader function tool. A Barclamp is a module component that implements functionality for Crowbar.
Core barclamps operate the essential functions of the Crowbar deployment mechanics while other barclamps extend the
system for specific applications.

**This functonality of this barclamp DOES NOT stand alone, the Crowbar Framework is required**

About this barclamp
-------------------

[![Build Status](https://travis-ci.org/crowbar/barclamp-raid.svg?branch=master)](https://travis-ci.org/crowbar/barclamp-raid)
[![Code Climate](https://codeclimate.com/github/crowbar/barclamp-raid/badges/gpa.svg)](https://codeclimate.com/github/crowbar/barclamp-raid)
[![Test Coverage](https://codeclimate.com/github/crowbar/barclamp-raid/badges/coverage.svg)](https://codeclimate.com/github/crowbar/barclamp-raid)
[![Dependency Status](https://gemnasium.com/crowbar/barclamp-raid.svg)](https://gemnasium.com/crowbar/barclamp-raid)

Information for this barclamp is maintained on the [Crowbar Framework Wiki](https://github.com/crowbar/crowbar/wiki)

Steps to setup
--------------

* Install SUSE Manager Server
* Inside SUSE Manager, create an activation key. The activation key will be used in the barclamp's WebUI.
* Download the `https://your-manager-server.example.com/pub/rhn-org-trusted-ssl-cert-*-*.noarch.rpm` file (check the
  version number) as `chef/cookbooks/raid/files/default/ssl-cert.rpm` (in this barclamp's directory tree).
* Reinstalling the barclamp might be required in order for crowbar to take notice of the new file. Do this with:
  `/opt/dell/bin/barclamp_install.rb --rpm raid`
* Now apply the barclamp from Crowbar's WebUI on selected nodes.

Legals
------

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
specific language governing permissions and limitations under the License.
