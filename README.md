# Perl5-Debugger-Multiline-Paste
Added Multi Line Paste feature to the PERL 5 debugger.
This adds support for multi line pasting of code into the interactive CLI debugger.
Install into /usr/lib/perl5/<YOUR_LIB_DIRECTORY>
Start the debugger.
To enter the multiline mode type   "PASTEMODE"
 Enter your multiline code..
To stop multiline mode type "ENDPASTE"

Example:

$ perl -de1

Loading DB routines from perl5db.pl version 1.51
Editor support available.

Enter h or 'h h' for help, or 'man perldebug' for more help.

main::(-e:1):   1
  DB<1>

  DB<1>

  DB<1> @lines = qw( this is a test)

  DB<2> PASTEMODE
foreach $elem(@lines){
 print "$elem";
}
ENDPASTE
thisisatest





