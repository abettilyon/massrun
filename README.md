Massrun was written by Allen Bettilyon <allen@bettilyon.net>
Copywrite Allen Bettilyon

-------------------------------------------------------------------------------

Massrun is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

Massrun is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

For a copy of the GNU General Public License, see http://www.gnu.org/licenses
or, write to the Free Software Foundation, Inc. 

   59 Temple Place 
   Suite 330 
   Boston, MA 02111-1307  USA 

--------------------------------------------------------------------------------

Massrun is a tool used for running commands accross large clusters of machines.
It is based on the notion of host classes which are defined by modifitying the
%classes hash inside the perl code.  The hash is simpley a list of class names
and they're cooresponding list file.  Each listfile is a simple TXT file with
one hostname per line, and using the pound (#) symbol as comments.

The massrun command attempts to run ssh commands accross each node listed in 
the classes.  It is strongly suggested that you have host keys already configured
accross all the nodes so that you can run ssh commands without having to enter
in passwords, or accept host keys.  

Massrun has the ability to run the commands serially, or in parallel.  Simply
add the --parallel commandline argument to the command to run in parallel.


  massrun --class=foo --cmd=uptime --parallel

-------------------------------------------------------------------------------

Feel free to conctact me with any questions, comments, suggeststions or
concerns about massrun.  I can be reached at allen@bettilyon.net, and would 
love to hear from you.









