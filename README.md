#Jinjer


Jinjer is a command-line tool to render Jinja 2 templates easily.

##Usage

jinjer [options] TEMPLATE-FILE

TEMPLATE-FILE is the name of the template file to be rendered. It's loaded by
Jinja, using the parameter -t if specified as the templates directory to be
sarched for.

Parameters to the template can be passed in two ways:

- in the command line, as pairs of KEY VALUE:


    jinjer template.tpl x 1 y 2

- in a separate yaml file, specified with -p PARAMETER-FILE:


    jinjer template.tpl -p parameters.yml

Output is printed by default to standard output, unless an output file is
specified with -o OUTPUT-FILE:

    jinjer template.tpl -o output.txt

##License

Copyright(c) 2013 André Roque Matheus. Jinjer is MIT licensed, see LICENSE.txt
for license rights and limitations.