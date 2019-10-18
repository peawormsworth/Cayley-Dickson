CayleyDickson.pm
====================

A classic quantum state emulator using Cayley-Dickson algebra

Install using CPAN:

     $ perl -MCPAN -e 'install CayleyDickson'

Sample Usage:

    my $quaternion1 = CayleyDickson->new(-1,0,1,0);
    my $quaternion2 = CayleyDickson->new(1,2,3,4);

    my $product    = $quaternion1 * $quaternion2;
    my $division   = $quaternion1 / $quaternion2;
    my $sum        = $quaternion1 + $quaternion2;
    my $difference = $quaternion1 - $quaternion2;
    
    my $complex =  CayleyDickson->new(1,-1);
    my $octonion = $complex->tensor($quaternion1);

    my $unit_octonion = $octonion / $octonion

Status:

    Standard Cayley-Dickson constructions using the Pt3 doubling product in common use has been tested.
    Complex, Quaternion, Octonion, Sedenion math operations (+,-,*,/) and tensor products are functional.

    Other doubling products remain to be verified.
    Dual, Split and Bi-complex numbers will be added soon.

Warning:

    This is a work in progress. Some things may not work.
    Please double check your Sedonion calculations by hand before depending on this program.

Locations:

    This project is available on ...
      MetaCPAN: https://metacpan.org/pod/CayleyDickson
      GitHub: https://github.com/peawormsworth/CayleyDickson


COPYRIGHT AND LICENSE

    Copyright (C) 2019 by Jeff Anderson

see individual license in each package under LICENSE


