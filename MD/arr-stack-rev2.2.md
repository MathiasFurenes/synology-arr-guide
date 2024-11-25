       How to install a full ARR-stack on Synology NAS running DSM 7.2     <!-- /\* Font Definitions \*/ @font-face {font-family:Helvetica; panose-1:2 11 6 4 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Courier; panose-1:2 7 4 9 2 2 5 2 4 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-format:other; mso-font-pitch:fixed; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Tms Rmn"; panose-1:2 2 6 3 4 5 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-format:other; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Helv; panose-1:2 11 6 4 2 2 2 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-format:other; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"New York"; panose-1:2 4 5 3 6 5 6 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:System; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-format:other; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Wingdings; panose-1:5 0 0 0 0 0 0 0 0 0; mso-font-charset:2; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"MS Mincho"; panose-1:2 2 6 9 4 2 5 8 3 4; mso-font-alt:"\\FF2D\\FF33 \\660E\\671D"; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:Batang; panose-1:2 3 6 0 0 1 1 1 1 1; mso-font-alt:\\BC14\\D0D5; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:SimSun; panose-1:2 1 6 0 3 1 1 1 1 1; mso-font-alt:\\5B8B\\4F53; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:515 680460288 22 0 262145 0;} @font-face {font-family:PMingLiU; panose-1:2 1 6 1 0 1 1 1 1 1; mso-font-alt:\\65B0\\7D30\\660E\\9AD4; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610611969 684719354 22 0 1048577 0;} @font-face {font-family:"MS Gothic"; panose-1:2 11 6 9 7 2 5 8 2 4; mso-font-alt:"\\FF2D\\FF33 \\30B4\\30B7\\30C3\\30AF"; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:Dotum; panose-1:2 11 6 0 0 1 1 1 1 1; mso-font-alt:\\B3CB\\C6C0; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:SimHei; panose-1:2 1 6 0 3 1 1 1 1 1; mso-font-alt:\\9ED1\\4F53; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147482945 953122042 22 0 262145 0;} @font-face {font-family:MingLiU; panose-1:2 1 6 9 0 1 1 1 1 1; mso-font-alt:\\7D30\\660E\\9AD4; mso-font-charset:136; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610611969 684719354 22 0 1048577 0;} @font-face {font-family:Mincho; panose-1:2 2 6 9 4 3 5 8 3 5; mso-font-alt:\\660E\\671D; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:fixed; mso-font-signature:1 134676480 16 0 131072 0;} @font-face {font-family:Gulim; panose-1:2 11 6 0 0 1 1 1 1 1; mso-font-alt:\\AD74\\B9BC; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:Century; panose-1:2 4 6 4 5 5 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Angsana New"; panose-1:2 2 6 3 5 4 5 2 3 4; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:"Cordia New"; panose-1:2 11 3 4 2 2 2 2 2 4; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Mangal; panose-1:0 0 4 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:32771 0 0 0 1 0;} @font-face {font-family:Latha; panose-1:2 0 4 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1048579 0 0 0 1 0;} @font-face {font-family:Sylfaen; panose-1:1 10 5 2 5 3 6 3 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:67110535 0 0 0 159 0;} @font-face {font-family:Vrinda; panose-1:0 0 4 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:65539 0 0 0 1 0;} @font-face {font-family:Raavi; panose-1:2 0 5 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:131075 0 0 0 1 0;} @font-face {font-family:Shruti; panose-1:2 0 5 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:262147 0 0 0 1 0;} @font-face {font-family:Sendnya; panose-1:0 0 4 0 0 0 0 0 0 0; mso-font-charset:1; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 0 0 0 0 0;} @font-face {font-family:Gautami; panose-1:2 0 5 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:2097155 0 0 0 1 0;} @font-face {font-family:Tunga; panose-1:0 0 4 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:4194307 0 0 0 1 0;} @font-face {font-family:"Estrangelo Edessa"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:1; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 0 0 0 0 0;} @font-face {font-family:"Cambria Math"; panose-1:2 4 5 3 5 4 6 3 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536869121 1107305727 33554432 0 415 0;} @font-face {font-family:"Yu Gothic"; panose-1:2 11 4 0 0 0 0 0 0 0; mso-font-alt:\\6E38\\30B4\\30B7\\30C3\\30AF; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:DengXian; panose-1:2 1 6 0 3 1 1 1 1 1; mso-font-alt:\\7B49\\7EBF; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612033 953122042 22 0 262159 0;} @font-face {font-family:Calibri; panose-1:2 15 5 2 2 2 4 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1040178053 9 0 511 0;} @font-face {font-family:"Calibri Light"; panose-1:2 15 3 2 2 2 4 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1040178053 9 0 511 0;} @font-face {font-family:"Palatino Linotype"; panose-1:2 4 5 2 5 5 5 3 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536870265 1073741843 0 0 415 0;} @font-face {font-family:Verdana; panose-1:2 11 6 4 3 5 4 4 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610610945 1073750107 16 0 415 0;} @font-face {font-family:"Arial Unicode MS"; panose-1:2 11 6 4 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Aptos Display"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:Aptos; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Segoe UI Emoji"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 134217728 0 1 0;} @font-face {font-family:Consolas; panose-1:2 11 6 9 2 2 4 3 2 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536869121 64767 1 0 415 0;} @font-face {font-family:inherit; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-alt:Cambria; mso-font-charset:0; mso-generic-font-family:roman; mso-font-format:other; mso-font-pitch:auto; mso-font-signature:0 0 0 0 0 0;} @font-face {font-family:Marlett; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:2; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Arial Black"; panose-1:2 11 10 4 2 1 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073772795 0 0 159 0;} @font-face {font-family:"Bahnschrift Light"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiLight"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:Bahnschrift; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiBold"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift Light SemiCondensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiLight SemiConde"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiCondensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiBold SemiConden"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift Light Condensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiLight Condensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift Condensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Bahnschrift SemiBold Condensed"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:Cambria; panose-1:2 4 5 3 5 4 6 3 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536869121 1107305727 33554432 0 415 0;} @font-face {font-family:Candara; panose-1:2 14 5 2 3 3 3 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1073783883 0 0 415 0;} @font-face {font-family:"Candara Light"; panose-1:2 14 5 2 3 3 3 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611969 2 0 0 415 0;} @font-face {font-family:"Comic Sans MS"; panose-1:3 15 7 2 3 3 2 2 2 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:647 19 0 0 159 0;} @font-face {font-family:Constantia; panose-1:2 3 6 2 5 3 6 3 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:Corbel; panose-1:2 11 5 3 2 2 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1073783883 0 0 415 0;} @font-face {font-family:"Corbel Light"; panose-1:2 11 3 3 2 2 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1073783883 0 0 415 0;} @font-face {font-family:Ebrima; panose-1:2 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612641 33554497 2048 0 147 0;} @font-face {font-family:"Franklin Gothic Medium"; panose-1:2 11 6 3 2 1 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:Gabriola; panose-1:4 4 6 5 5 16 2 2 13 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:-536870161 1342185547 0 0 159 0;} @font-face {font-family:Gadugi; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 12288 0 1 0;} @font-face {font-family:Georgia; panose-1:2 4 5 2 5 4 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"HoloLens MDL2 Assets"; panose-1:5 10 1 2 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 268435456 0 0 1 0;} @font-face {font-family:Impact; panose-1:2 11 8 6 3 9 2 5 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Ink Free"; panose-1:3 8 4 2 0 5 0 0 0 0; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:536872591 1073741834 0 0 415 0;} @font-face {font-family:"Javanese Text"; panose-1:2 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Leelawadee UI"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1560281085 0 65536 0 65793 0;} @font-face {font-family:"Leelawadee UI Semilight"; panose-1:2 11 4 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1560281085 0 65536 0 65793 0;} @font-face {font-family:"Lucida Console"; panose-1:2 11 6 9 4 5 4 2 2 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147482993 6144 0 0 31 0;} @font-face {font-family:"Lucida Sans Unicode"; panose-1:2 11 6 2 3 5 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147480833 14699 0 0 191 0;} @font-face {font-family:"Malgun Gothic"; panose-1:2 11 5 3 2 0 0 2 0 4; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1879048145 701988091 18 0 524289 0;} @font-face {font-family:"\\@Malgun Gothic"; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1879048145 701988091 18 0 524289 0;} @font-face {font-family:"Malgun Gothic Semilight"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1342174545 165641467 18 0 4063677 0;} @font-face {font-family:"\\@Malgun Gothic Semilight"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1342174545 165641467 18 0 4063677 0;} @font-face {font-family:"Microsoft Himalaya"; panose-1:1 1 1 0 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 65536 64 0 1 0;} @font-face {font-family:"Microsoft JhengHei"; panose-1:2 11 6 4 3 5 4 4 2 4; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:679 684672000 22 0 1048585 0;} @font-face {font-family:"\\@Microsoft JhengHei"; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:679 684672000 22 0 1048585 0;} @font-face {font-family:"Microsoft JhengHei UI"; panose-1:2 11 6 4 3 5 4 4 2 4; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:679 684672000 22 0 1048585 0;} @font-face {font-family:"\\@Microsoft JhengHei UI"; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:679 684672000 22 0 1048585 0;} @font-face {font-family:"Microsoft JhengHei Light"; panose-1:2 11 3 4 3 5 4 4 2 4; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482969 684672000 22 0 1048585 0;} @font-face {font-family:"\\@Microsoft JhengHei Light"; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482969 684672000 22 0 1048585 0;} @font-face {font-family:"Microsoft JhengHei UI Light"; panose-1:2 11 3 4 3 5 4 4 2 4; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482969 684672000 22 0 1048585 0;} @font-face {font-family:"\\@Microsoft JhengHei UI Light"; mso-font-charset:136; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482969 684672000 22 0 1048585 0;} @font-face {font-family:"Microsoft New Tai Lue"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 -2147483648 0 1 0;} @font-face {font-family:"Microsoft PhagsPa"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 134217728 0 1 0;} @font-face {font-family:"Microsoft Sans Serif"; panose-1:2 11 6 4 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-452972801 -1073717157 41 0 66047 0;} @font-face {font-family:"Microsoft Tai Le"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 1073741824 0 1 0;} @font-face {font-family:"Microsoft YaHei"; panose-1:2 11 5 3 2 2 4 2 2 4; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718224464 22 0 262175 0;} @font-face {font-family:"\\@Microsoft YaHei"; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718224464 22 0 262175 0;} @font-face {font-family:"Microsoft YaHei UI"; panose-1:2 11 5 3 2 2 4 2 2 4; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718224464 22 0 262175 0;} @font-face {font-family:"\\@Microsoft YaHei UI"; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718224464 22 0 262175 0;} @font-face {font-family:"Microsoft YaHei Light"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718209040 22 0 262175 0;} @font-face {font-family:"\\@Microsoft YaHei Light"; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718209040 22 0 262175 0;} @font-face {font-family:"Microsoft YaHei UI Light"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718209040 22 0 262175 0;} @font-face {font-family:"\\@Microsoft YaHei UI Light"; mso-font-charset:134; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 718209040 22 0 262175 0;} @font-face {font-family:"Microsoft Yi Baiti"; panose-1:3 0 5 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483645 66562 524290 0 1 0;} @font-face {font-family:MingLiU-ExtB; panose-1:2 2 5 0 0 0 0 0 0 0; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:"\\@MingLiU-ExtB"; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:PMingLiU-ExtB; panose-1:2 2 5 0 0 0 0 0 0 0; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:"\\@PMingLiU-ExtB"; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:MingLiU\_HKSCS-ExtB; panose-1:2 2 5 0 0 0 0 0 0 0; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:"\\@MingLiU\_HKSCS-ExtB"; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:"Mongolian Baiti"; panose-1:3 0 5 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483613 0 131072 0 1 0;} @font-face {font-family:"\\@MS Gothic"; panose-1:2 11 6 9 7 2 5 8 2 4; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"MS UI Gothic"; panose-1:2 11 6 0 7 2 5 8 2 4; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"\\@MS UI Gothic"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"MS PGothic"; panose-1:2 11 6 0 7 2 5 8 2 4; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"\\@MS PGothic"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"MV Boli"; panose-1:2 0 5 0 3 2 0 9 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 256 0 1 0;} @font-face {font-family:"Myanmar Text"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 1024 0 1 0;} @font-face {font-family:"Nirmala UI"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130739165 33554506 512 0 1 0;} @font-face {font-family:"Nirmala UI Semilight"; panose-1:2 11 4 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130739165 33554506 512 0 1 0;} @font-face {font-family:"Sans Serif Collection"; panose-1:2 11 5 2 4 5 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2146983741 33579072 688914433 0 1 0;} @font-face {font-family:"Segoe Fluent Icons"; panose-1:5 10 1 2 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 268435456 0 0 1 0;} @font-face {font-family:"Segoe MDL2 Assets"; panose-1:5 10 1 2 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 268435456 0 0 1 0;} @font-face {font-family:"Segoe Print"; panose-1:2 0 6 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:655 0 0 0 159 0;} @font-face {font-family:"Segoe Script"; panose-1:3 11 5 4 2 0 0 0 0 3; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:655 0 0 0 159 0;} @font-face {font-family:"Segoe UI"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe UI Black"; panose-1:2 11 10 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1073800319 33 0 415 0;} @font-face {font-family:"Segoe UI Historic"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483153 33554434 6340736 0 1 0;} @font-face {font-family:"Segoe UI Light"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe UI Semibold"; panose-1:2 11 7 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe UI Semilight"; panose-1:2 11 4 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe UI Symbol"; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483165 302055407 262144 0 1 0;} @font-face {font-family:"Segoe UI Variable Small Light"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Small Semilig"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Small"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Small Semibol"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Text Light"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Text Semiligh"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Text"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Text Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Display Light"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Display Semil"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Display"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Variable Display Semib"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"\\@SimSun"; panose-1:2 1 6 0 3 1 1 1 1 1; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:515 680460288 22 0 262145 0;} @font-face {font-family:NSimSun; panose-1:2 1 6 9 3 1 1 1 1 1; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:515 680460288 22 0 262145 0;} @font-face {font-family:"\\@NSimSun"; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:515 680460288 22 0 262145 0;} @font-face {font-family:SimSun-ExtB; panose-1:2 1 6 9 6 1 1 1 1 1; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 168689664 16 0 262145 0;} @font-face {font-family:"\\@SimSun-ExtB"; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 168689664 16 0 262145 0;} @font-face {font-family:"Sitka Small"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Small Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Text"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Text Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Subheading"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Subheading Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Heading"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Heading Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Display"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Display Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Banner"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:"Sitka Banner Semibold"; panose-1:0 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611985 1073750091 0 0 415 0;} @font-face {font-family:Tahoma; panose-1:2 11 6 4 3 5 4 4 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520081665 -1073717157 41 0 66047 0;} @font-face {font-family:"Trebuchet MS"; panose-1:2 11 6 3 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1671 0 0 0 159 0;} @font-face {font-family:Webdings; panose-1:5 3 1 2 1 5 9 6 7 3; mso-font-charset:2; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"\\@Yu Gothic"; panose-1:2 11 4 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic UI"; panose-1:2 11 5 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic UI"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic UI Semibold"; panose-1:2 11 7 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic UI Semibold"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic Light"; panose-1:2 11 3 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic Light"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic UI Light"; panose-1:2 11 3 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic UI Light"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic Medium"; panose-1:2 11 5 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic Medium"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Yu Gothic UI Semilight"; panose-1:2 11 4 0 0 0 0 0 0 0; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"\\@Yu Gothic UI Semilight"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717749759 22 0 131231 0;} @font-face {font-family:"Agency FB"; panose-1:2 11 5 3 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Algerian; panose-1:4 2 7 5 4 10 2 6 7 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Book Antiqua"; panose-1:2 4 6 2 5 3 5 3 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Arial Narrow"; panose-1:2 11 6 6 2 2 2 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 2048 0 0 159 0;} @font-face {font-family:"Arial Rounded MT Bold"; panose-1:2 15 7 4 3 5 4 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Baskerville Old Face"; panose-1:2 2 6 2 8 5 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bauhaus 93"; panose-1:4 3 9 5 2 11 2 2 12 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bell MT"; panose-1:2 2 5 3 6 3 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bernard MT Condensed"; panose-1:2 5 8 6 6 9 5 2 4 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bodoni MT"; panose-1:2 7 6 3 8 6 6 2 2 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bodoni MT Black"; panose-1:2 7 10 3 8 6 6 2 2 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bodoni MT Condensed"; panose-1:2 7 6 6 8 6 6 2 2 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bodoni MT Poster Compressed"; panose-1:2 7 7 6 8 6 1 5 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:7 0 0 0 17 0;} @font-face {font-family:"Bookman Old Style"; panose-1:2 5 6 4 5 5 5 2 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Bradley Hand ITC"; panose-1:3 7 4 2 5 3 2 3 2 3; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Britannic Bold"; panose-1:2 11 9 3 6 7 3 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Berlin Sans FB"; panose-1:2 14 6 2 2 5 2 2 3 6; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Berlin Sans FB Demi"; panose-1:2 14 8 2 2 5 2 2 3 6; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Broadway; panose-1:4 4 9 5 8 11 2 2 5 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Brush Script MT"; panose-1:3 6 8 2 4 4 6 7 3 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Bookshelf Symbol 7"; panose-1:5 1 1 1 1 1 1 1 1 1; mso-font-charset:2; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Californian FB"; panose-1:2 7 4 3 6 8 11 3 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Calisto MT"; panose-1:2 4 6 3 5 5 5 3 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Castellar; panose-1:2 10 4 2 6 4 6 1 3 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Century Schoolbook"; panose-1:2 4 6 4 5 5 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:Centaur; panose-1:2 3 5 4 5 2 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Chiller; panose-1:4 2 4 4 3 16 7 2 6 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Colonna MT"; panose-1:4 2 8 5 6 2 2 3 2 3; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Cooper Black"; panose-1:2 8 9 4 4 3 11 2 4 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Copperplate Gothic Bold"; panose-1:2 14 7 5 2 2 6 2 4 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Copperplate Gothic Light"; panose-1:2 14 5 7 2 2 6 2 4 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Curlz MT"; panose-1:4 4 4 4 5 7 2 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Dubai; panose-1:2 11 5 3 3 4 3 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475353 -2147483648 8 0 65 0;} @font-face {font-family:"Dubai Light"; panose-1:2 11 3 3 3 4 3 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475353 -2147483648 8 0 65 0;} @font-face {font-family:"Dubai Medium"; panose-1:2 11 6 3 3 4 3 3 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475353 -2147483648 8 0 65 0;} @font-face {font-family:Elephant; panose-1:2 2 9 4 9 5 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Engravers MT"; panose-1:2 9 7 7 8 5 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Eras Bold ITC"; panose-1:2 11 9 7 3 5 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Eras Demi ITC"; panose-1:2 11 8 5 3 5 4 2 8 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Eras Light ITC"; panose-1:2 11 4 2 3 5 4 2 8 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Eras Medium ITC"; panose-1:2 11 6 2 3 5 4 2 8 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Felix Titling"; panose-1:4 6 5 5 6 2 2 2 10 4; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Forte; panose-1:3 6 9 2 4 5 2 7 2 3; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Franklin Gothic Book"; panose-1:2 11 5 3 2 1 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Franklin Gothic Demi"; panose-1:2 11 7 3 2 1 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Franklin Gothic Demi Cond"; panose-1:2 11 7 6 3 4 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Franklin Gothic Heavy"; panose-1:2 11 9 3 2 1 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Franklin Gothic Medium Cond"; panose-1:2 11 6 6 3 4 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Freestyle Script"; panose-1:3 8 4 2 3 2 5 11 4 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"French Script MT"; panose-1:3 2 4 2 4 6 7 4 6 5; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Footlight MT Light"; panose-1:2 4 6 2 6 3 10 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Garamond; panose-1:2 2 4 4 3 3 1 1 8 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:Gigi; panose-1:4 4 5 4 6 16 7 2 13 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Gill Sans MT"; panose-1:2 11 5 2 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Gill Sans MT Condensed"; panose-1:2 11 5 6 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Gill Sans Ultra Bold Condensed"; panose-1:2 11 10 6 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Gill Sans Ultra Bold"; panose-1:2 11 10 2 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Gloucester MT Extra Condensed"; panose-1:2 3 8 8 2 6 1 1 1 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Gill Sans MT Ext Condensed Bold"; panose-1:2 11 9 2 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Century Gothic"; panose-1:2 11 5 2 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Goudy Old Style"; panose-1:2 2 5 2 5 3 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Goudy Stout"; panose-1:2 2 9 4 7 3 11 2 4 1; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Harlow Solid Italic"; panose-1:4 3 6 4 2 15 2 2 13 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Harrington; panose-1:4 4 5 5 5 10 2 2 7 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Haettenschweiler; panose-1:2 11 7 6 4 9 2 6 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"High Tower Text"; panose-1:2 4 5 2 5 5 6 3 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Imprint MT Shadow"; panose-1:4 2 6 5 6 3 3 3 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Informal Roman"; panose-1:3 6 4 2 3 4 6 11 2 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Blackadder ITC"; panose-1:4 2 5 5 5 16 7 2 13 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Edwardian Script ITC"; panose-1:3 3 3 2 4 7 7 13 8 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Kristen ITC"; panose-1:3 5 5 2 4 2 2 3 2 2; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Jokerman; panose-1:4 9 6 5 6 13 6 2 7 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Juice ITC"; panose-1:4 4 4 3 4 10 2 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Kunstler Script"; panose-1:3 3 4 2 2 6 7 13 13 6; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Wide Latin"; panose-1:2 10 10 7 5 5 5 2 4 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Lucida Bright"; panose-1:2 4 6 2 5 5 5 2 3 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Lucida Calligraphy"; panose-1:3 1 1 1 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Leelawadee; panose-1:2 11 5 2 4 2 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777219 0 0 0 65537 0;} @font-face {font-family:"Lucida Fax"; panose-1:2 6 6 2 5 5 5 2 2 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Lucida Handwriting"; panose-1:3 1 1 1 1 1 1 1 1 1; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Lucida Sans"; panose-1:2 11 6 2 3 5 4 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Lucida Sans Typewriter"; panose-1:2 11 5 9 3 5 4 3 2 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Magneto; panose-1:4 3 8 5 5 8 2 2 13 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Maiandra GD"; panose-1:2 14 5 2 3 3 8 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Matura MT Script Capitals"; panose-1:3 2 8 2 6 6 2 7 2 2; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Mistral; panose-1:3 9 7 2 3 4 7 2 4 3; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Modern No\\. 20"; panose-1:2 7 7 4 7 5 5 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Microsoft Uighur"; panose-1:2 0 0 0 0 0 0 0 0 0; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147475421 -2147483646 8 0 65 0;} @font-face {font-family:"Monotype Corsiva"; panose-1:3 1 1 1 1 2 1 1 1 1; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"MT Extra"; panose-1:5 5 1 2 1 2 5 2 2 2; mso-font-charset:2; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Niagara Engraved"; panose-1:4 2 5 2 7 7 3 3 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Niagara Solid"; panose-1:4 2 5 2 7 7 2 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"OCR A Extended"; panose-1:2 1 5 9 2 1 2 1 3 3; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Old English Text MT"; panose-1:3 4 9 2 4 5 8 3 8 6; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Onyx; panose-1:4 5 6 2 8 7 2 2 2 3; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"MS Outlook"; panose-1:5 1 1 0 1 0 0 0 0 0; mso-font-charset:2; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Palace Script MT"; panose-1:3 3 3 2 2 6 7 12 11 5; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Papyrus; panose-1:3 7 5 2 6 5 2 3 2 5; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Parchment; panose-1:3 4 6 2 4 7 8 4 8 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Perpetua; panose-1:2 2 5 2 6 4 1 2 3 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Perpetua Titling MT"; panose-1:2 2 5 2 6 5 5 2 8 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Playbill; panose-1:4 5 6 3 10 6 2 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Poor Richard"; panose-1:2 8 5 2 5 5 5 2 7 2; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Pristina; panose-1:3 6 4 2 4 4 6 8 2 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Rage Italic"; panose-1:3 7 5 2 4 5 7 7 3 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Ravie; panose-1:4 4 8 5 5 8 9 2 6 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"MS Reference Sans Serif"; panose-1:2 11 6 4 3 5 4 4 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 0 0 0 415 0;} @font-face {font-family:"MS Reference Specialty"; panose-1:5 0 5 0 0 0 0 0 0 0; mso-font-charset:2; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Rockwell Condensed"; panose-1:2 6 6 3 5 4 5 2 1 4; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Rockwell; panose-1:2 6 6 3 2 2 5 2 4 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Rockwell Extra Bold"; panose-1:2 6 9 3 4 5 5 2 4 3; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Script MT Bold"; panose-1:3 4 6 2 4 6 7 8 9 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Showcard Gothic"; panose-1:4 2 9 4 2 1 2 2 6 4; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Snap ITC"; panose-1:4 4 10 7 6 10 2 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Stencil; panose-1:4 4 9 5 13 8 2 2 4 4; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Tw Cen MT"; panose-1:2 11 6 2 2 1 4 2 6 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Tw Cen MT Condensed"; panose-1:2 11 6 6 2 1 4 2 2 3; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Tw Cen MT Condensed Extra Bold"; panose-1:2 11 8 3 2 2 2 2 2 4; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Tempus Sans ITC"; panose-1:4 2 4 4 3 13 7 2 2 2; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Viner Hand ITC"; panose-1:3 7 5 2 3 5 2 2 2 3; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Vivaldi; panose-1:3 2 6 2 5 5 6 9 8 4; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Vladimir Script"; panose-1:3 5 4 2 4 4 7 7 3 5; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Wingdings 2"; panose-1:5 2 1 2 1 5 7 7 7 7; mso-font-charset:2; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Wingdings 3"; panose-1:5 4 1 2 1 8 7 7 7 7; mso-font-charset:2; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:SimSun-ExtG; panose-1:2 1 6 9 6 1 1 1 1 1; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 168689664 16 0 262145 0;} @font-face {font-family:"\\@SimSun-ExtG"; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 168689664 16 0 262145 0;} @font-face {font-family:"Cascadia Code ExtraLight"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Code Light"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Code SemiLight"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Code"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Code SemiBold"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Mono ExtraLight"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Mono Light"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Mono SemiLight"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Mono"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:"Cascadia Mono SemiBold"; panose-1:2 11 6 9 2 0 0 2 0 4; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1593824513 -1040123397 262176 0 511 0;} @font-face {font-family:Abadi; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Abadi Extra Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:Abel; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Abril Fatface"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612569 1342185563 0 0 147 0;} @font-face {font-family:"ADLaM Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147475345 1107296330 0 0 1 0;} @font-face {font-family:Aharoni; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Al Fresco"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483473 268435530 0 0 3 0;} @font-face {font-family:"Alasassy Caps"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Aldhabi; mso-font-charset:178; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147475449 -2147483648 8 0 65 0;} @font-face {font-family:Alef; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741824 0 0 179 0;} @font-face {font-family:Aleo; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 0 0 131 0;} @font-face {font-family:"Aleo Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 0 0 131 0;} @font-face {font-family:"Amasis MT Pro"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612561 1073750107 0 0 147 0;} @font-face {font-family:"Amasis MT Pro Black"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612561 1073750107 0 0 147 0;} @font-face {font-family:"Amasis MT Pro Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612561 1073750107 0 0 147 0;} @font-face {font-family:"Amasis MT Pro Medium"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612561 1073750107 0 0 147 0;} @font-face {font-family:"Amatic SC"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536873487 1073741826 0 0 439 0;} @font-face {font-family:AngsanaUPC; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Anton; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750139 0 0 403 0;} @font-face {font-family:Aparajita; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:32771 0 0 0 1 0;} @font-face {font-family:"Aptos Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos Narrow"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"Aptos Serif"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1592449281 -1073681157 65536 0 415 0;} @font-face {font-family:"Arabic Typesetting"; mso-font-charset:178; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147475449 -2147483648 8 0 211 0;} @font-face {font-family:"Aref Ruqaa"; mso-font-charset:178; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147475345 -2147483573 0 0 65 0;} @font-face {font-family:"Arial Nova"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:655 2 0 0 415 0;} @font-face {font-family:"Arial Nova Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:655 2 0 0 415 0;} @font-face {font-family:"Arial Nova Cond Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:655 2 0 0 415 0;} @font-face {font-family:"Arial Nova Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:655 2 0 0 415 0;} @font-face {font-family:Assistant; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610433 1073750091 0 0 33 0;} @font-face {font-family:"Assistant ExtraBold"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610433 1073750091 0 0 33 0;} @font-face {font-family:"Assistant ExtraLight"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610433 1073750091 0 0 33 0;} @font-face {font-family:"Assistant Light"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610433 1073750091 0 0 33 0;} @font-face {font-family:"Assistant SemiBold"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610433 1073750091 0 0 33 0;} @font-face {font-family:Athiti; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Athiti ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Athiti Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Athiti Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Athiti SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Avenir Next LT Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483409 1342185546 0 0 147 0;} @font-face {font-family:"Avenir Next LT Pro Demi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483409 1342185546 0 0 147 0;} @font-face {font-family:"Avenir Next LT Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612497 1342185547 0 0 147 0;} @font-face {font-family:"Baguet Script"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:Barlow; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Condensed Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed ExLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Semi Condensed Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Barlow Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:BatangChe; mso-font-charset:129; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:"Bebas Neue"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:Bembo; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:Bierstadt; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Bierstadt Display"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:BierstadtAlt; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"BierstadtAlt2 Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"BierstadtAlt3 Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:"BierstadtAlt4 Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:BierstadtAlt5; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:Biome; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1592449281 -2147483638 65536 0 415 0;} @font-face {font-family:"Biome Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1592449281 -2147483638 65536 0 415 0;} @font-face {font-family:"Boucherie Block"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 0 0 3 0;} @font-face {font-family:"Boucherie Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483473 268443722 0 0 1 0;} @font-face {font-family:"Browallia New"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:BrowalliaUPC; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:"Buxton Sketch"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750235 0 0 159 0;} @font-face {font-family:"Caveat Brush"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342185563 0 0 147 0;} @font-face {font-family:Cavolini; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-1592449281 -2147483638 65536 0 415 0;} @font-face {font-family:"Chamberi Super Display"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:Charmonman; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Chilgok Gwon Anja"; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483409 152518731 16 0 2621441 0;} @font-face {font-family:"Chilgok Kim Yeongbun"; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483409 152518731 16 0 2621441 0;} @font-face {font-family:"Chilgok Lee Jonghui"; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483409 152518731 16 0 2621441 0;} @font-face {font-family:"Chilgok Lee Wonsun"; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483409 152518731 16 0 2621441 0;} @font-face {font-family:Chonburi; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Cochocib Script Latin Pro"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612561 1342177354 0 0 147 0;} @font-face {font-family:"Concert One"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483609 67 0 0 273 0;} @font-face {font-family:Cond; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:536871559 3 0 0 415 0;} @font-face {font-family:Congenial; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268443739 0 0 1 0;} @font-face {font-family:"Congenial Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268443739 0 0 1 0;} @font-face {font-family:"Congenial Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268443739 0 0 1 0;} @font-face {font-family:"Congenial SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268443739 0 0 1 0;} @font-face {font-family:"Congenial UltraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268443739 0 0 1 0;} @font-face {font-family:Convection; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342177354 0 0 159 0;} @font-face {font-family:"Convection Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 145 0;} @font-face {font-family:"Convection Extra Bold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342177354 0 0 159 0;} @font-face {font-family:"Convection Symbol"; mso-font-charset:2; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:0 268435456 0 0 -2147483648 0;} @font-face {font-family:"Convection UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483473 1342177354 0 0 155 0;} @font-face {font-family:CordiaUPC; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Dante; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:DaunPenh; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 65536 0 1 0;} @font-face {font-family:David; mso-font-charset:177; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:Daytona; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482897 10 0 0 415 0;} @font-face {font-family:"Daytona Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Daytona Condensed Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Daytona Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"DengXian Light"; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612033 953122042 22 0 262159 0;} @font-face {font-family:"Didact Gothic"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1610613455 2 0 0 415 0;} @font-face {font-family:DilleniaUPC; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:"DM Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"DM Mono Light"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"DM Mono Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"DM Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 1342185563 0 0 147 0;} @font-face {font-family:"DM Sans Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 1342185563 0 0 147 0;} @font-face {font-family:"DM Serif Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483537 75 0 0 415 0;} @font-face {font-family:"DM Serif Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483537 75 0 0 415 0;} @font-face {font-family:DokChampa; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2097151997 0 0 0 65537 0;} @font-face {font-family:Dosis; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:"Dosis ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:"Dosis ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:"Dosis Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:"Dosis Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:"Dosis SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1073750139 0 0 147 0;} @font-face {font-family:DotumChe; mso-font-charset:129; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:"Dreaming Outloud Pro"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483409 10 8 0 1 0;} @font-face {font-family:"Dreaming Outloud Script Pro"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483409 10 8 0 1 0;} @font-face {font-family:"EB Garamond"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 33555475 0 0 415 0;} @font-face {font-family:"EB Garamond ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 33555475 0 0 415 0;} @font-face {font-family:"EB Garamond Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 33555475 0 0 415 0;} @font-face {font-family:"EB Garamond SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 33555475 0 0 415 0;} @font-face {font-family:"Elephant Pro"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871559 2 0 0 415 0;} @font-face {font-family:EucrosiaUPC; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Euphemia; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483537 74 8192 0 1 0;} @font-face {font-family:Fahkwang; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Fahkwang ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Fahkwang Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Fahkwang Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Fahkwang SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Fairwater Script"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612689 268435531 0 0 1 0;} @font-face {font-family:"Fairwater Script Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612689 268435531 0 0 1 0;} @font-face {font-family:FangSong; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147482945 953122042 22 0 262145 0;} @font-face {font-family:"Fave Script Bold Pro"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 1342177354 0 0 403 0;} @font-face {font-family:"Fira Code"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870161 302053627 8 0 159 0;} @font-face {font-family:"Fira Code Light"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870161 302053627 8 0 159 0;} @font-face {font-family:"Fira Code Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870161 302053627 8 0 159 0;} @font-face {font-family:"Fira Code Retina"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870161 302053627 8 0 159 0;} @font-face {font-family:"Fira Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:1073742471 33568769 0 0 159 0;} @font-face {font-family:"Fira Mono Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:1073742471 33568769 0 0 159 0;} @font-face {font-family:"Fira Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Condensed Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Extra Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Extra Condensed Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Extra Condensed Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Extra Condensed Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fira Sans Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613503 1 0 0 415 0;} @font-face {font-family:"Fjalla One"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483457 1073741899 0 0 1 0;} @font-face {font-family:"Forte Forward"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342201931 8 0 147 0;} @font-face {font-family:"Frank Ruhl Libre"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741825 0 0 163 0;} @font-face {font-family:"Frank Ruhl Libre Black"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741825 0 0 163 0;} @font-face {font-family:"Frank Ruhl Libre Light"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741825 0 0 163 0;} @font-face {font-family:"Frank Ruhl Libre Medium"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741825 0 0 163 0;} @font-face {font-family:FrankRuehl; mso-font-charset:177; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Fredoka One"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 1073741898 0 0 1 0;} @font-face {font-family:FreesiaUPC; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Gabriela; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:515 0 0 0 5 0;} @font-face {font-family:Gaegu; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 17825794 16 0 1 0;} @font-face {font-family:"Gaegu Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 17825794 16 0 1 0;} @font-face {font-family:"Georgia Pro"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Black"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Cond"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Cond Black"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Cond Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Cond Semibold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Georgia Pro Semibold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482961 3 0 0 159 0;} @font-face {font-family:"Gill Sans Nova"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Cond Lt"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Cond Ultra Bold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Cond XBd"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:"Gill Sans Nova Ultra Bold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 159 0;} @font-face {font-family:Gisha; mso-font-charset:177; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147481593 1073741890 0 0 33 0;} @font-face {font-family:"Goudy Type"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:Grandview; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:"Grandview Display"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612025 2 0 0 415 0;} @font-face {font-family:Grotesque; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Grotesque Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:GulimChe; mso-font-charset:129; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:Gungsuh; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:GungsuhChe; mso-font-charset:129; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1342176593 1775729915 48 0 524447 0;} @font-face {font-family:"Hadassah Friedlaender"; mso-font-charset:177; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Hammersmith One"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612561 1073750090 0 0 147 0;} @font-face {font-family:Heebo; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:"Heebo Black"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:"Heebo ExtraBold"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:"Heebo Light"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:"Heebo Medium"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:"Heebo Thin"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610610457 1073741891 0 0 33 0;} @font-face {font-family:HGGothicE; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGMaruGothicMPRO; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGMinchoE; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGPGothicE; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGPMinchoE; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGPSoeiKakugothicUB; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGSGothicE; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGSMinchoE; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGSoeiKakugothicUB; mso-font-charset:128; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:HGSSoeiKakugothicUB; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 717745662 18 0 131073 0;} @font-face {font-family:Hind; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Hind Colombo"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 512 0 147 0;} @font-face {font-family:"Hind Colombo Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 512 0 147 0;} @font-face {font-family:"Hind Colombo Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 512 0 147 0;} @font-face {font-family:"Hind Colombo SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 512 0 147 0;} @font-face {font-family:"Hind Guntur"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2097159 0 0 0 147 0;} @font-face {font-family:"Hind Guntur Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2097159 0 0 0 147 0;} @font-face {font-family:"Hind Guntur Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2097159 0 0 0 147 0;} @font-face {font-family:"Hind Guntur SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2097159 0 0 0 147 0;} @font-face {font-family:"Hind Jalandhar"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:131079 0 0 0 147 0;} @font-face {font-family:"Hind Jalandhar Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:131079 0 0 0 147 0;} @font-face {font-family:"Hind Jalandhar Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:131079 0 0 0 147 0;} @font-face {font-family:"Hind Jalandhar SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:131079 0 0 0 147 0;} @font-face {font-family:"Hind Kochi"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:8388615 0 0 0 147 0;} @font-face {font-family:"Hind Kochi Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:8388615 0 0 0 147 0;} @font-face {font-family:"Hind Kochi Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:8388615 0 0 0 147 0;} @font-face {font-family:"Hind Kochi SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:8388615 0 0 0 147 0;} @font-face {font-family:"Hind Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Hind Madurai"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1048583 0 0 0 147 0;} @font-face {font-family:"Hind Madurai Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1048583 0 0 0 147 0;} @font-face {font-family:"Hind Madurai Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1048583 0 0 0 147 0;} @font-face {font-family:"Hind Madurai SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1048583 0 0 0 147 0;} @font-face {font-family:"Hind Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Hind Mysuru"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:4194307 0 0 0 147 0;} @font-face {font-family:"Hind Mysuru Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:4194307 0 0 0 147 0;} @font-face {font-family:"Hind Mysuru Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:4194307 0 0 0 147 0;} @font-face {font-family:"Hind Mysuru SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:4194307 0 0 0 147 0;} @font-face {font-family:"Hind SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Hind Siliguri"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:65543 0 0 0 147 0;} @font-face {font-family:"Hind Siliguri Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:65543 0 0 0 147 0;} @font-face {font-family:"Hind Siliguri Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:65543 0 0 0 147 0;} @font-face {font-family:"Hind Siliguri SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:65543 0 0 0 147 0;} @font-face {font-family:"Hind Vadodara"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:262151 0 0 0 147 0;} @font-face {font-family:"Hind Vadodara Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:262151 0 0 0 147 0;} @font-face {font-family:"Hind Vadodara Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:262151 0 0 0 147 0;} @font-face {font-family:"Hind Vadodara SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:262151 0 0 0 147 0;} @font-face {font-family:"IBM Plex Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Mono ExtraLight"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Mono Light"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Mono Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Mono SemiBold"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Mono Thin"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610612113 1342185595 0 0 407 0;} @font-face {font-family:"IBM Plex Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Sans Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612625 1342185595 0 0 403 0;} @font-face {font-family:"IBM Plex Sans Condensed Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612625 1342185595 0 0 403 0;} @font-face {font-family:"IBM Plex Sans Condensed Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612625 1342185595 0 0 403 0;} @font-face {font-family:"IBM Plex Sans Condensed Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612625 1342185595 0 0 403 0;} @font-face {font-family:"IBM Plex Sans ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Sans Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Sans Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Sans Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185595 0 0 415 0;} @font-face {font-family:"IBM Plex Serif"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:"IBM Plex Serif ExtraLight"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:"IBM Plex Serif Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:"IBM Plex Serif Medium"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:"IBM Plex Serif SemiBold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:"IBM Plex Serif Thin"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610612113 1342185531 0 0 407 0;} @font-face {font-family:Inconsolata; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Condensed SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Expanded SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraCondensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraCondensed Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraExpanded"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraExpanded Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraExpanded Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraExpanded Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiCondensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiCondensed Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiCondensed Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiCondensed Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiExpanded"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiExpanded Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiExpanded Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiExpanded Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata SemiExpanded Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraCondensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraCondensed Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraExpanded"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraExpanded Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraExpanded Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:"Inconsolata UltraExpanded Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:IrisUPC; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:"Iskoola Pota"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 512 0 1 0;} @font-face {font-family:Italianno; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 0 0 147 0;} @font-face {font-family:JasmineUPC; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:"Josefin Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Josefin Sans Bold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Josefin Sans Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Josefin Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Josefin Sans Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Josefin Slab"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 4 0 0 17 0;} @font-face {font-family:"Josefin Slab Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 4 0 0 17 0;} @font-face {font-family:"Josefin Slab SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 4 0 0 17 0;} @font-face {font-family:"Josefin Slab Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 4 0 0 17 0;} @font-face {font-family:Jumble; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 268435530 0 0 1 0;} @font-face {font-family:KaiTi; mso-font-charset:134; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147482945 953122042 22 0 262145 0;} @font-face {font-family:Kalinga; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:Karla; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750107 0 0 147 0;} @font-face {font-family:"Karla ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750107 0 0 147 0;} @font-face {font-family:"Karla ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750107 0 0 147 0;} @font-face {font-family:"Karla Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750107 0 0 147 0;} @font-face {font-family:"Karla Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750107 0 0 147 0;} @font-face {font-family:"Karla Tamil Inclined"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2146435037 134217794 335544320 0 1 0;} @font-face {font-family:"Karla Tamil Upright"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2146435037 134217794 335544320 0 1 0;} @font-face {font-family:Kartika; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:8388611 0 0 0 1 0;} @font-face {font-family:Kermit; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extrabold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extrabold Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extrabold Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extralight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extralight Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Extralight Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Light Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Light Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Semibold Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Semibold Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Thin Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Kermit Thin Expanded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482961 1342185546 0 0 415 0;} @font-face {font-family:"Khmer UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 65536 0 1 0;} @font-face {font-family:Kigelia; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-535484673 -1040187317 67584 0 415 0;} @font-face {font-family:"Kigelia Arabic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610603905 -2147483645 8 0 479 0;} @font-face {font-family:"Kigelia Arabic Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610603905 -2147483645 8 0 479 0;} @font-face {font-family:"Kigelia Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-535484673 -1040187317 67584 0 415 0;} @font-face {font-family:"Klee One"; mso-font-charset:128; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 1791491327 82 0 1179653 0;} @font-face {font-family:"Klee One SemiBold"; mso-font-charset:128; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 1791491327 82 0 1179653 0;} @font-face {font-family:KodchiangUPC; mso-font-charset:222; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Kokila; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:32771 0 0 0 1 0;} @font-face {font-family:Krub; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Krub ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Krub Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Krub Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Krub SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:Lalezar; mso-font-charset:178; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536879111 0 8 0 467 0;} @font-face {font-family:"Lao UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2113929213 0 0 0 1 0;} @font-face {font-family:Lato; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Lato Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-520092929 1342237951 33 0 415 0;} @font-face {font-family:"Levenim MT"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Libre Barcode 128"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode 128 Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode 39"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode 39 Extended"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode 39 Extended Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode 39 Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Libre Barcode EAN13 Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483609 0 0 0 1 0;} @font-face {font-family:"Libre Baskerville"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612545 1342177371 0 0 147 0;} @font-face {font-family:"Libre Franklin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:"Libre Franklin Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750107 0 0 403 0;} @font-face {font-family:Ligconsolata; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 63979 32 0 403 0;} @font-face {font-family:LilyUPC; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130706429 0 0 0 65537 0;} @font-face {font-family:Livvic; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:"Livvic Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1073750091 0 0 403 0;} @font-face {font-family:Lobster; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 1 0 0 407 0;} @font-face {font-family:"Lobster Two"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 1073741898 0 0 1 0;} @font-face {font-family:Lora; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 151 0;} @font-face {font-family:"Lora Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 151 0;} @font-face {font-family:"Mangal Pro"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32771 0 0 0 1 0;} @font-face {font-family:Meddon; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612561 1342185546 0 0 147 0;} @font-face {font-family:Meiryo; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791492095 134217746 0 131231 0;} @font-face {font-family:"Meiryo UI"; mso-font-charset:128; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1791492095 134217746 0 131231 0;} @font-face {font-family:Merriweather; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 2 0 0 407 0;} @font-face {font-family:"Merriweather Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 2 0 0 407 0;} @font-face {font-family:"Merriweather Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 2 0 0 407 0;} @font-face {font-family:"Merriweather Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611457 1073750139 0 0 403 0;} @font-face {font-family:"Merriweather Sans ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611457 1073750139 0 0 403 0;} @font-face {font-family:"Merriweather Sans Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611457 1073750139 0 0 403 0;} @font-face {font-family:"Microsoft GothicNeo"; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482945 701998203 16 0 2687135 0;} @font-face {font-family:"Microsoft GothicNeo Light"; mso-font-charset:129; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147482945 701998203 16 0 2687135 0;} @font-face {font-family:MingLiU\_HKSCS; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610611969 684719354 22 0 1048577 0;} @font-face {font-family:MingLiU\_MSCS; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482881 684719354 22 0 1048577 0;} @font-face {font-family:MingLiU\_MSCS-ExtB; mso-font-charset:136; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 168296456 16 0 1048577 0;} @font-face {font-family:Miriam; mso-font-charset:177; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Miriam Fixed"; mso-font-charset:177; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Miriam Libre"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741824 0 0 179 0;} @font-face {font-family:Mitr; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Mitr ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Mitr Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Mitr Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Mitr SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Modern Love"; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Modern Love Caps"; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Modern Love Grunge"; mso-font-charset:0; mso-generic-font-family:decorative; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:Montserrat; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:"Montserrat Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 3 0 0 407 0;} @font-face {font-family:MoolBoran; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 65536 0 1 0;} @font-face {font-family:"Mr Gabe"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"MS PMincho"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536870145 1791491579 134217746 0 131231 0;} @font-face {font-family:"Mystical Woods Rough Script"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870927 268435456 0 0 147 0;} @font-face {font-family:"Mystical Woods Smooth Script"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870927 268435456 0 0 147 0;} @font-face {font-family:"Nanum Brush Script"; mso-font-charset:129; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 165149947 16 0 524289 0;} @font-face {font-family:"Nanum Pen"; mso-font-charset:129; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 165149931 16 0 524289 0;} @font-face {font-family:NanumGothic; mso-font-charset:129; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 165149931 16 0 524289 0;} @font-face {font-family:NanumGothicCoding; mso-font-charset:129; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147482969 702020859 16 0 524301 0;} @font-face {font-family:NanumGothicExtraBold; mso-font-charset:129; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 165149931 16 0 524289 0;} @font-face {font-family:NanumMyeongjo; mso-font-charset:129; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 165149931 16 0 524289 0;} @font-face {font-family:NanumMyeongjoExtraBold; mso-font-charset:129; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 165149931 16 0 524289 0;} @font-face {font-family:Narkisim; mso-font-charset:177; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Neue Haas Grotesk Text Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"News Gothic MT"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Nina; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:647 0 0 0 159 0;} @font-face {font-family:"Nirmala Text"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130739165 33554506 512 0 1 0;} @font-face {font-family:"Nirmala Text Semilight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2130739165 33554506 512 0 1 0;} @font-face {font-family:"Nordique Inline"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Noto Music"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 33579008 16777216 0 1 0;} @font-face {font-family:"Noto Nastaliq Urdu"; mso-font-charset:178; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 -2147475392 0 0 65 0;} @font-face {font-family:"Noto Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536837377 1073772799 33 0 415 0;} @font-face {font-family:"Noto Sans AnatoHiero"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Avestan"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Bassa Vah"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Batak"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Bhaiksuki"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Brahmi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Buginese"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Buhid"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 1048576 0 1 0;} @font-face {font-family:"Noto Sans Carian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans CaucAlban"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:67 33562624 1 0 1 0;} @font-face {font-family:"Noto Sans Chakma"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147418109 33562624 1024 0 1 0;} @font-face {font-family:"Noto Sans Coptic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483197 33562624 1 0 1 0;} @font-face {font-family:"Noto Sans Cuneiform"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Cypriot"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Deseret"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 8388608 0 1 0;} @font-face {font-family:"Noto Sans Devanagari"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari UI Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari UI Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari UI Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Devanagari UI Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450845 8262 0 0 1 0;} @font-face {font-family:"Noto Sans Duployan"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans EgyptHiero"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Elbasan"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:195 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Elymaic"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Glagolitic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:579 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Gothic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:67 33554432 4194304 0 1 0;} @font-face {font-family:"Noto Sans Grantha"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2146402301 33562628 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gujarati UI Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147188733 8258 0 0 1 0;} @font-face {font-family:"Noto Sans Gunjala Gondi"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 33562688 0 0 1 0;} @font-face {font-family:"Noto Sans Hanunoo"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 1048576 0 1 0;} @font-face {font-family:"Noto Sans Hatran"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans ImpAramaic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Indic Siyaq Numbers"; mso-font-charset:178; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:8195 33554432 0 0 65 0;} @font-face {font-family:"Noto Sans InsPahlavi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans InsParthi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Javanese"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Kaithi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Kharoshthi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Khojki"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147221501 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Khudawadi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Lepcha"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Limbu"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 8192 536870912 0 1 0;} @font-face {font-family:"Noto Sans Linear A"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Linear B"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Lycian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Lydian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Mahajani"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Mandaic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Manichaean"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 33562624 134217728 0 1 0;} @font-face {font-family:"Noto Sans Marchen"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Masaram Gondi"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147450877 33562688 0 0 1 0;} @font-face {font-family:"Noto Sans Math"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483453 33580268 33554448 0 1 0;} @font-face {font-family:"Noto Sans Mayan Numerals"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Mende Kikakui"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Meroitic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Miao"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Modi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Mongolian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33629184 131074 0 1 0;} @font-face {font-family:"Noto Sans Mro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Multani"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:131075 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Myanmar"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar Blk"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar ExtBd"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar ExtLt"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar Med"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar SemBd"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Myanmar UI Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Sans Nabataean"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Newa"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483581 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans NewTaiLue"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 -2147483648 0 1 0;} @font-face {font-family:"Noto Sans NKo"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 -2147475456 0 0 1 0;} @font-face {font-family:"Noto Sans Nushu"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Ogham"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 16384 0 1 0;} @font-face {font-family:"Noto Sans Old Italic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 2097152 0 1 0;} @font-face {font-family:"Noto Sans Old Permic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:579 33562628 0 0 1 0;} @font-face {font-family:"Noto Sans Old Turkic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans OldHung"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Noto Sans OldNorArab"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans OldPersian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans OldSogdian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans OldSouArab"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya Blk"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya UI"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya UI Blk"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Oriya UI Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:524291 0 0 0 1 0;} @font-face {font-family:"Noto Sans Osage"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:67 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Osmanya"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Pahawh Hmong"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Palmyrene"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans PauCinHau"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans PhagsPa"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 73728 134348800 0 1 0;} @font-face {font-family:"Noto Sans Phoenician"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans PsaPahlavi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Rejang"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Runic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 32768 0 1 0;} @font-face {font-family:"Noto Sans Samaritan"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 0 0 0 1 0;} @font-face {font-family:"Noto Sans Saurashtra"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Sharada"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Shavian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Siddham"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Sogdian"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475453 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Soyombo"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Syloti Nagri"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147385341 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Symbols2"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33612772 262176 0 1 0;} @font-face {font-family:"Noto Sans Syriac"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475389 24640 128 0 1 0;} @font-face {font-family:"Noto Sans Syriac Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475389 24640 128 0 1 0;} @font-face {font-family:"Noto Sans Syriac Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147475389 24640 128 0 1 0;} @font-face {font-family:"Noto Sans Tagalog"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 1048576 0 1 0;} @font-face {font-family:"Noto Sans Tagbanwa"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 1048576 0 1 0;} @font-face {font-family:"Noto Sans Tai Le"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483581 73728 1073742848 0 1 0;} @font-face {font-family:"Noto Sans Tai Viet"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612733 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Takri"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Tamil Supplement"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1048579 0 0 0 1 0;} @font-face {font-family:"Noto Sans Thai Looped Black"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Bold"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped ExtLight"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Extrabold"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Light"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Medium"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Regular"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Semibold"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Thai Looped Thin"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777217 0 0 0 65536 0;} @font-face {font-family:"Noto Sans Tifinagh"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483581 8192 0 0 1 0;} @font-face {font-family:"Noto Sans Tirhuta"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147385341 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans Ugaritic"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Vai"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Noto Sans Wancho"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33562624 0 0 1 0;} @font-face {font-family:"Noto Sans WarangCiti"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483645 33554432 0 0 1 0;} @font-face {font-family:"Noto Sans Yi"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 327680 524304 0 1 0;} @font-face {font-family:"Noto Sans Zanabazar"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Serif"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-536870145 1342208255 41 0 415 0;} @font-face {font-family:"Noto Serif Ahom"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 33562624 0 0 1 0;} @font-face {font-family:"Noto Serif Balinese"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 0 0 1 0;} @font-face {font-family:"Noto Serif Dogra"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147450877 33562624 0 0 1 0;} @font-face {font-family:"Noto Serif Grantha"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2146402301 33562628 0 0 1 0;} @font-face {font-family:"Noto Serif Myanmar"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar Blk"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar ExtBd"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar ExtLt"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar Med"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar SemBd"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Myanmar Thin"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483645 8192 134218752 0 1 0;} @font-face {font-family:"Noto Serif Tangut"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Noto Traditional Nushu"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 167772160 0 0 1 0;} @font-face {font-family:Nunito; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:"Nunito SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185547 0 0 407 0;} @font-face {font-family:Nyala; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612625 0 2048 0 147 0;} @font-face {font-family:OCRB; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:"Open Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870161 1073750107 40 0 415 0;} @font-face {font-family:"Open Sans ExtraBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870161 1073750107 40 0 415 0;} @font-face {font-family:"Open Sans Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870161 1073750107 40 0 415 0;} @font-face {font-family:"Open Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870161 1073750107 40 0 415 0;} @font-face {font-family:Oranienbaum; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483089 10 0 0 151 0;} @font-face {font-family:Oswald; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 0 0 0 407 0;} @font-face {font-family:"Oswald ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 0 0 0 407 0;} @font-face {font-family:"Oswald Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 0 0 0 407 0;} @font-face {font-family:"Oswald Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 0 0 0 407 0;} @font-face {font-family:"Oswald SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871439 0 0 0 407 0;} @font-face {font-family:Oxygen; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750091 0 0 147 0;} @font-face {font-family:"Oxygen Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483537 1073750089 0 0 1 0;} @font-face {font-family:"Oxygen Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-2147483601 8266 0 0 147 0;} @font-face {font-family:Pacifico; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 2 0 0 407 0;} @font-face {font-family:Palanquin; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Palanquin ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Palanquin Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Palanquin Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Palanquin SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Palanquin Thin"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147450705 1342185546 0 0 147 0;} @font-face {font-family:"Patrick Hand"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Patrick Hand SC"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536870919 0 0 0 403 0;} @font-face {font-family:"Petit Formal Script"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-1610612545 1342177371 0 0 147 0;} @font-face {font-family:"Plantagenet Cherokee"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:3 0 4096 0 1 0;} @font-face {font-family:"Playfair Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 0 0 0 407 0;} @font-face {font-family:"Playfair Display Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 0 0 0 407 0;} @font-face {font-family:"Playfair Display SC"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 0 0 0 407 0;} @font-face {font-family:"Playfair Display SC Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 0 0 0 407 0;} @font-face {font-family:"Poiret One"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536871431 2 0 0 407 0;} @font-face {font-family:Poppins; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:"Poppins Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:32775 0 0 0 147 0;} @font-face {font-family:Posterama; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1592449281 -805298101 65536 0 415 0;} @font-face {font-family:Pridi; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Pridi ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Pridi Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Pridi Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Pridi SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:Prompt; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt Black"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt ExtraBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Prompt Thin"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"PT Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-1610611985 1342208235 0 0 151 0;} @font-face {font-family:"PT Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185547 0 0 151 0;} @font-face {font-family:"PT Sans Caption"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185547 0 0 151 0;} @font-face {font-family:"PT Sans Narrow"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185547 0 0 151 0;} @font-face {font-family:"PT Serif"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185547 0 0 151 0;} @font-face {font-family:"PT Serif Caption"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610611985 1342185547 0 0 151 0;} @font-face {font-family:Quattrocento; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483457 1073741899 0 0 1 0;} @font-face {font-family:"Quattrocento Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483457 1073741915 0 0 1 0;} @font-face {font-family:Questrial; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536870145 1073750047 134217769 0 403 0;} @font-face {font-family:"Quire Sans"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1592449281 -2147483638 65536 0 415 0;} @font-face {font-family:"Quire Sans Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Quire Sans Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:Raleway; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Raleway Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 1342185563 0 0 407 0;} @font-face {font-family:"Rastanty Cortez"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483609 268435530 0 0 1 0;} @font-face {font-family:"Reem Kufi"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:3 0 0 0 1 0;} @font-face {font-family:Roboto; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Condensed"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Condensed Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Condensed Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Roboto Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 268443739 32 0 415 0;} @font-face {font-family:"Roboto Mono Light"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 268443739 32 0 415 0;} @font-face {font-family:"Roboto Mono Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 268443739 32 0 415 0;} @font-face {font-family:"Roboto Mono Thin"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 268443739 32 0 415 0;} @font-face {font-family:"Roboto Serif 20pt"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Serif 20pt Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1593835265 1342203515 0 0 403 0;} @font-face {font-family:"Roboto Slab"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Slab Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1279 -2147467169 34 0 415 0;} @font-face {font-family:"Roboto Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-536868097 1342185855 33 0 415 0;} @font-face {font-family:"Rockwell Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 0 0 0 15 0;} @font-face {font-family:"Rockwell Nova"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 415 0;} @font-face {font-family:"Rockwell Nova Cond"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 415 0;} @font-face {font-family:"Rockwell Nova Cond Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 415 0;} @font-face {font-family:"Rockwell Nova Extra Bold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 415 0;} @font-face {font-family:"Rockwell Nova Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483001 2 0 0 415 0;} @font-face {font-family:Rod; mso-font-charset:177; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:2051 0 0 0 33 0;} @font-face {font-family:"Sabon Next LT"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1592449281 -805306357 65536 0 415 0;} @font-face {font-family:Sacramento; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073741898 0 0 147 0;} @font-face {font-family:Sagona; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Sagona Book"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Sagona ExtraLight"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Sakkal Majalla"; mso-font-charset:178; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147475449 -2147483648 8 0 211 0;} @font-face {font-family:"Sanskrit Text"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-1610579897 0 0 0 1 0;} @font-face {font-family:Seaford; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Seaford Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Secular One"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741824 0 0 179 0;} @font-face {font-family:"Segoe Marker"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 1073750091 0 0 1 0;} @font-face {font-family:"Segoe Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Display"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Display Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Display Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Display SemiLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Pro SemiLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-1610612049 1073750107 0 0 159 0;} @font-face {font-family:"Segoe Sans Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Hairline"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Display Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Hairline"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Small Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Hairline"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Sans Text Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-469750017 -1073683329 9 0 511 0;} @font-face {font-family:"Segoe Serif Banner"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Banner Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Banner Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Banner Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Display Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Display Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Display Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Text"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Text Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Text Semibold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe Serif Text Semilight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610611969 11 0 0 415 0;} @font-face {font-family:"Segoe UI Emoji L"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 33554432 0 0 1 0;} @font-face {font-family:"Segoe Xbox Symbol"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:3 301989888 0 0 1 0;} @font-face {font-family:Selawik; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"Selawik Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"Selawik Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:7 0 0 0 147 0;} @font-face {font-family:"Shadows Into Light Two"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612561 1342177354 0 0 147 0;} @font-face {font-family:"Shonar Bangla"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:65539 0 0 0 1 0;} @font-face {font-family:"Simplified Arabic"; mso-font-charset:178; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:8195 -2147483648 8 0 65 0;} @font-face {font-family:"Simplified Arabic Fixed"; mso-font-charset:178; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:8195 0 8 0 65 0;} @font-face {font-family:Skeena; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Skeena Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Source Code Pro"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Code Pro Black"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Code Pro ExtraLight"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Code Pro Light"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Code Pro Medium"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Code Pro Semibold"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:536871671 33568771 0 0 415 0;} @font-face {font-family:"Source Sans Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613495 33554433 0 0 415 0;} @font-face {font-family:"Source Sans Pro Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613495 33554433 0 0 415 0;} @font-face {font-family:"Source Sans Pro ExtraLight"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613495 33554433 0 0 415 0;} @font-face {font-family:"Source Sans Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613495 33554433 0 0 415 0;} @font-face {font-family:"Source Sans Pro SemiBold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:1610613495 33554433 0 0 415 0;} @font-face {font-family:"Source Serif Pro"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:536871559 33554435 0 0 415 0;} @font-face {font-family:"Source Serif Pro Black"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:536871559 33554435 0 0 415 0;} @font-face {font-family:"Source Serif Pro ExtraLight"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:536871559 33554435 0 0 415 0;} @font-face {font-family:"Source Serif Pro Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:536871559 33554435 0 0 415 0;} @font-face {font-family:"Source Serif Pro SemiBold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:536871559 33554435 0 0 415 0;} @font-face {font-family:"Speak Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Speak Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:Staatliches; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612497 1073750091 0 0 147 0;} @font-face {font-family:STCaiyun; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1 953090296 22 0 262145 0;} @font-face {font-family:STFangsong; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:647 135200768 16 0 262303 0;} @font-face {font-family:STHupo; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1 135200768 16 0 262144 0;} @font-face {font-family:STKaiti; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:647 135200768 16 0 262303 0;} @font-face {font-family:STXihei; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:647 135200768 16 0 262303 0;} @font-face {font-family:STXingkai; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1 135200768 16 0 262144 0;} @font-face {font-family:STXinwei; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:1 135200768 16 0 262144 0;} @font-face {font-family:STZhongsong; mso-font-charset:134; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:647 135200768 16 0 262303 0;} @font-face {font-family:"Suez One"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:2055 1073741824 0 0 179 0;} @font-face {font-family:Tenorite; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"Tenorite Display"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147483645 1 0 0 1 0;} @font-face {font-family:"TH SarabunPSK"; mso-font-charset:222; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:16777219 0 0 0 65809 0;} @font-face {font-family:"The Hand"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Hand Black"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Hand Extrablack"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Hand Light"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Serif Hand"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Serif Hand Black"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Serif Hand Extrablack"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"The Serif Hand Light"; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Tisa Offc Serif Pro"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147482905 2 0 0 415 0;} @font-face {font-family:"Tisa Offc Serif Pro Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-2147482905 2 0 0 415 0;} @font-face {font-family:"Titillium Web"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:"Titillium Web Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:"Titillium Web ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:"Titillium Web Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:"Titillium Web SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:7 1 0 0 147 0;} @font-face {font-family:"Trade Gothic Inline"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next Heavy"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next HvyCd"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Trade Gothic Next Rounded"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Traditional Arabic"; mso-font-charset:178; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:8195 -2147483648 8 0 65 0;} @font-face {font-family:Trirong; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong Black"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong ExtraBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong ExtraLight"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong Light"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong Medium"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong SemiBold"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:"Trirong Thin"; mso-font-charset:222; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:553648135 1 0 0 65939 0;} @font-face {font-family:Ubuntu; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1342185563 0 0 159 0;} @font-face {font-family:"Ubuntu Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1342185563 0 0 159 0;} @font-face {font-family:"Ubuntu Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1342185563 0 0 159 0;} @font-face {font-family:"Ubuntu Medium"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-536870145 1342185563 0 0 159 0;} @font-face {font-family:"Ubuntu Mono"; mso-font-charset:0; mso-generic-font-family:modern; mso-font-pitch:fixed; mso-font-signature:-536870145 1342185563 0 0 159 0;} @font-face {font-family:"UD Digi Kyokasho N-B"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:"UD Digi Kyokasho N-R"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:"UD Digi Kyokasho NK-B"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:"UD Digi Kyokasho NK-R"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:"UD Digi Kyokasho NP-B"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:"UD Digi Kyokasho NP-R"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482973 717745402 16 0 131072 0;} @font-face {font-family:Univers; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 0 0 0 15 0;} @font-face {font-family:"Univers Condensed"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 0 0 0 15 0;} @font-face {font-family:"Univers Condensed Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 0 0 0 15 0;} @font-face {font-family:"Univers Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 0 0 0 15 0;} @font-face {font-family:"Urdu Typesetting"; mso-font-charset:178; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:8195 -2147483648 8 0 65 0;} @font-face {font-family:Utsaah; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:32771 0 0 0 1 0;} @font-face {font-family:Vani; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:2097155 0 0 0 1 0;} @font-face {font-family:"Varela Round"; mso-font-charset:177; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:536872967 3 0 0 435 0;} @font-face {font-family:"Verdana Pro"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Cond"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Cond Black"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Cond Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Cond Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Light"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:"Verdana Pro Semibold"; mso-font-charset:0; mso-generic-font-family:swiss; mso-font-pitch:variable; mso-font-signature:-2147483001 67 0 0 159 0;} @font-face {font-family:Vijaya; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:1048579 0 0 0 1 0;} @font-face {font-family:"Walbaum Display"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Walbaum Display Heavy"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Walbaum Display Light"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Walbaum Display SemiBold"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Walbaum Heading"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:"Walbaum Text"; mso-font-charset:0; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147483601 10 0 0 1 0;} @font-face {font-family:Wandohope; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482897 165117179 16 0 655365 0;} @font-face {font-family:"Work Sans"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans Black"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans ExtraBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans ExtraLight"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans Light"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans Medium"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans SemiBold"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:"Work Sans Thin"; mso-font-charset:0; mso-generic-font-family:auto; mso-font-pitch:variable; mso-font-signature:-1610612481 1342234747 0 0 403 0;} @font-face {font-family:Yesteryear; mso-font-charset:0; mso-generic-font-family:script; mso-font-pitch:variable; mso-font-signature:-1610612497 1073741898 0 0 147 0;} @font-face {font-family:"Yu Mincho"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482905 717749503 18 0 131231 0;} @font-face {font-family:"Yu Mincho Demibold"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482905 717749503 18 0 131231 0;} @font-face {font-family:"Yu Mincho Light"; mso-font-charset:128; mso-generic-font-family:roman; mso-font-pitch:variable; mso-font-signature:-2147482905 717749503 18 0 131231 0;} /\* Style Definitions \*/ p.MsoNormal, li.MsoNormal, div.MsoNormal {mso-style-unhide:no; mso-style-qformat:yes; mso-style-parent:""; margin-top:0cm; margin-right:0cm; margin-bottom:8.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} h1 {mso-style-priority:9; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Overskrift 1 Tegn"; mso-style-next:Normal; margin-top:18.0pt; margin-right:0cm; margin-bottom:4.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:1; font-size:20.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal;} h2 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 2 Tegn"; mso-style-next:Normal; margin-top:8.0pt; margin-right:0cm; margin-bottom:4.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:2; font-size:16.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal;} h3 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 3 Tegn"; mso-style-next:Normal; margin-top:8.0pt; margin-right:0cm; margin-bottom:4.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:3; font-size:14.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal;} h4 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 4 Tegn"; mso-style-next:Normal; margin-top:4.0pt; margin-right:0cm; margin-bottom:2.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:4; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal; font-style:italic;} h5 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 5 Tegn"; mso-style-next:Normal; margin-top:4.0pt; margin-right:0cm; margin-bottom:2.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:5; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal;} h6 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 6 Tegn"; mso-style-next:Normal; margin-top:2.0pt; margin-right:0cm; margin-bottom:0cm; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:6; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:normal; font-style:italic;} p.MsoHeading7, li.MsoHeading7, div.MsoHeading7 {mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 7 Tegn"; mso-style-next:Normal; margin-top:2.0pt; margin-right:0cm; margin-bottom:0cm; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:7; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoHeading8, li.MsoHeading8, div.MsoHeading8 {mso-style-noshow:yes; mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 8 Tegn"; mso-style-next:Normal; margin:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:8; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#272727; mso-themecolor:text1; mso-themetint:216; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-style:italic;} p.MsoHeading9, li.MsoHeading9, div.MsoHeading9 {mso-style-noshow:yes; mso-style-priority:9; mso-style-qformat:yes; mso-style-link:"Overskrift 9 Tegn"; mso-style-next:Normal; margin:0cm; line-height:115%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; mso-outline-level:9; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#272727; mso-themecolor:text1; mso-themetint:216; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc1, li.MsoToc1, div.MsoToc1 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:6.0pt; margin-right:0cm; margin-bottom:6.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan; font-size:10.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; text-transform:uppercase; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-weight:bold;} p.MsoToc2, li.MsoToc2, div.MsoToc2 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:12.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:10.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; font-variant:small-caps; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc3, li.MsoToc3, div.MsoToc3 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:24.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:10.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-style:italic;} p.MsoToc4, li.MsoToc4, div.MsoToc4 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:36.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc5, li.MsoToc5, div.MsoToc5 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:48.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc6, li.MsoToc6, div.MsoToc6 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:60.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc7, li.MsoToc7, div.MsoToc7 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:72.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc8, li.MsoToc8, div.MsoToc8 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:84.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoToc9, li.MsoToc9, div.MsoToc9 {mso-style-update:auto; mso-style-priority:39; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:96.0pt; line-height:115%; mso-pagination:widow-orphan; font-size:9.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoHeader, li.MsoHeader, div.MsoHeader {mso-style-priority:99; mso-style-link:"Topptekst Tegn"; margin:0cm; mso-pagination:widow-orphan; tab-stops:center 8.0cm right 16.0cm; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoFooter, li.MsoFooter, div.MsoFooter {mso-style-priority:99; mso-style-link:"Bunntekst Tegn"; margin:0cm; mso-pagination:widow-orphan; tab-stops:center 8.0cm right 16.0cm; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoTitle, li.MsoTitle, div.MsoTitle {mso-style-priority:10; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Tittel Tegn"; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:4.0pt; margin-left:0cm; mso-add-space:auto; mso-pagination:widow-orphan; font-size:28.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; letter-spacing:-.5pt; mso-font-kerning:14.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoTitleCxSpFirst, li.MsoTitleCxSpFirst, div.MsoTitleCxSpFirst {mso-style-priority:10; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Tittel Tegn"; mso-style-next:Normal; mso-style-type:export-only; margin:0cm; mso-add-space:auto; mso-pagination:widow-orphan; font-size:28.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; letter-spacing:-.5pt; mso-font-kerning:14.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoTitleCxSpMiddle, li.MsoTitleCxSpMiddle, div.MsoTitleCxSpMiddle {mso-style-priority:10; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Tittel Tegn"; mso-style-next:Normal; mso-style-type:export-only; margin:0cm; mso-add-space:auto; mso-pagination:widow-orphan; font-size:28.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; letter-spacing:-.5pt; mso-font-kerning:14.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoTitleCxSpLast, li.MsoTitleCxSpLast, div.MsoTitleCxSpLast {mso-style-priority:10; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Tittel Tegn"; mso-style-next:Normal; mso-style-type:export-only; margin-top:0cm; margin-right:0cm; margin-bottom:4.0pt; margin-left:0cm; mso-add-space:auto; mso-pagination:widow-orphan; font-size:28.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; letter-spacing:-.5pt; mso-font-kerning:14.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoSubtitle, li.MsoSubtitle, div.MsoSubtitle {mso-style-priority:11; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Undertittel Tegn"; mso-style-next:Normal; margin-top:0cm; margin-right:0cm; margin-bottom:8.0pt; margin-left:0cm; line-height:115%; mso-pagination:widow-orphan; font-size:14.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166; letter-spacing:.75pt; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} a:link, span.MsoHyperlink {mso-style-priority:99; color:#467886; mso-themecolor:hyperlink; text-decoration:underline; text-underline:single;} a:visited, span.MsoHyperlinkFollowed {mso-style-noshow:yes; mso-style-priority:99; color:#96607D; mso-themecolor:followedhyperlink; text-decoration:underline; text-underline:single;} pre {mso-style-noshow:yes; mso-style-priority:99; mso-style-link:"HTML-forh�ndsformatert Tegn"; margin:0cm; margin-bottom:.0001pt; mso-pagination:widow-orphan; tab-stops:35.4pt; font-size:10.0pt; font-family:Consolas; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoNoSpacing, li.MsoNoSpacing, div.MsoNoSpacing {mso-style-priority:1; mso-style-unhide:no; mso-style-qformat:yes; mso-style-parent:""; mso-style-link:"Ingen mellomrom Tegn"; margin:0cm; mso-pagination:widow-orphan; font-size:11.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:minor-fareast; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi;} p.MsoListParagraph, li.MsoListParagraph, div.MsoListParagraph {mso-style-priority:34; mso-style-unhide:no; mso-style-qformat:yes; margin-top:0cm; margin-right:0cm; margin-bottom:8.0pt; margin-left:36.0pt; mso-add-space:auto; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoListParagraphCxSpFirst, li.MsoListParagraphCxSpFirst, div.MsoListParagraphCxSpFirst {mso-style-priority:34; mso-style-unhide:no; mso-style-qformat:yes; mso-style-type:export-only; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:36.0pt; mso-add-space:auto; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoListParagraphCxSpMiddle, li.MsoListParagraphCxSpMiddle, div.MsoListParagraphCxSpMiddle {mso-style-priority:34; mso-style-unhide:no; mso-style-qformat:yes; mso-style-type:export-only; margin-top:0cm; margin-right:0cm; margin-bottom:0cm; margin-left:36.0pt; mso-add-space:auto; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoListParagraphCxSpLast, li.MsoListParagraphCxSpLast, div.MsoListParagraphCxSpLast {mso-style-priority:34; mso-style-unhide:no; mso-style-qformat:yes; mso-style-type:export-only; margin-top:0cm; margin-right:0cm; margin-bottom:8.0pt; margin-left:36.0pt; mso-add-space:auto; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US;} p.MsoQuote, li.MsoQuote, div.MsoQuote {mso-style-priority:29; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Sitat Tegn"; mso-style-next:Normal; margin-top:8.0pt; margin-right:0cm; margin-bottom:8.0pt; margin-left:0cm; text-align:center; line-height:115%; mso-pagination:widow-orphan; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; color:#404040; mso-themecolor:text1; mso-themetint:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-style:italic;} p.MsoIntenseQuote, li.MsoIntenseQuote, div.MsoIntenseQuote {mso-style-priority:30; mso-style-unhide:no; mso-style-qformat:yes; mso-style-link:"Sterkt sitat Tegn"; mso-style-next:Normal; margin-top:18.0pt; margin-right:43.2pt; margin-bottom:18.0pt; margin-left:43.2pt; text-align:center; line-height:115%; mso-pagination:widow-orphan; border:none; mso-border-top-alt:solid #0F4761 .5pt; mso-border-top-themecolor:accent1; mso-border-top-themeshade:191; mso-border-bottom-alt:solid #0F4761 .5pt; mso-border-bottom-themecolor:accent1; mso-border-bottom-themeshade:191; padding:0cm; mso-padding-alt:10.0pt 0cm 10.0pt 0cm; font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; mso-font-kerning:1.0pt; mso-ligatures:standardcontextual; mso-fareast-language:EN-US; font-style:italic;} span.MsoIntenseEmphasis {mso-style-priority:21; mso-style-unhide:no; mso-style-qformat:yes; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; font-style:italic;} span.MsoIntenseReference {mso-style-priority:32; mso-style-unhide:no; mso-style-qformat:yes; font-variant:small-caps; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; letter-spacing:.25pt; font-weight:bold;} p.MsoTocHeading, li.MsoTocHeading, div.MsoTocHeading {mso-style-priority:39; mso-style-qformat:yes; mso-style-parent:"Overskrift 1"; mso-style-next:Normal; margin-top:12.0pt; margin-right:0cm; margin-bottom:0cm; margin-left:0cm; line-height:107%; mso-pagination:widow-orphan lines-together; page-break-after:avoid; font-size:16.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191;} span.Overskrift1Tegn {mso-style-name:"Overskrift 1 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 1"; mso-ansi-font-size:20.0pt; mso-bidi-font-size:20.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191;} span.Overskrift2Tegn {mso-style-name:"Overskrift 2 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 2"; mso-ansi-font-size:16.0pt; mso-bidi-font-size:16.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191;} span.Overskrift3Tegn {mso-style-name:"Overskrift 3 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 3"; mso-ansi-font-size:14.0pt; mso-bidi-font-size:14.0pt; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191;} span.Overskrift4Tegn {mso-style-name:"Overskrift 4 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 4"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; font-style:italic;} span.Overskrift5Tegn {mso-style-name:"Overskrift 5 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 5"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191;} span.Overskrift6Tegn {mso-style-name:"Overskrift 6 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 6"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166; font-style:italic;} span.Overskrift7Tegn {mso-style-name:"Overskrift 7 Tegn"; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 7"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166;} span.Overskrift8Tegn {mso-style-name:"Overskrift 8 Tegn"; mso-style-noshow:yes; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 8"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#272727; mso-themecolor:text1; mso-themetint:216; font-style:italic;} span.Overskrift9Tegn {mso-style-name:"Overskrift 9 Tegn"; mso-style-noshow:yes; mso-style-priority:9; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Overskrift 9"; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#272727; mso-themecolor:text1; mso-themetint:216;} span.TittelTegn {mso-style-name:"Tittel Tegn"; mso-style-priority:10; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:Tittel; mso-ansi-font-size:28.0pt; mso-bidi-font-size:28.0pt; font-family:"Aptos Display",sans-serif; mso-ascii-font-family:"Aptos Display"; mso-ascii-theme-font:major-latin; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-hansi-font-family:"Aptos Display"; mso-hansi-theme-font:major-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; letter-spacing:-.5pt; mso-font-kerning:14.0pt;} span.UndertittelTegn {mso-style-name:"Undertittel Tegn"; mso-style-priority:11; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:Undertittel; mso-ansi-font-size:14.0pt; mso-bidi-font-size:14.0pt; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:major-fareast; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:major-bidi; color:#595959; mso-themecolor:text1; mso-themetint:166; letter-spacing:.75pt;} span.SitatTegn {mso-style-name:"Sitat Tegn"; mso-style-priority:29; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:Sitat; color:#404040; mso-themecolor:text1; mso-themetint:191; font-style:italic;} span.SterktsitatTegn {mso-style-name:"Sterkt sitat Tegn"; mso-style-priority:30; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Sterkt sitat"; color:#0F4761; mso-themecolor:accent1; mso-themeshade:191; font-style:italic;} span.TopptekstTegn {mso-style-name:"Topptekst Tegn"; mso-style-priority:99; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:Topptekst;} span.BunntekstTegn {mso-style-name:"Bunntekst Tegn"; mso-style-priority:99; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:Bunntekst;} span.IngenmellomromTegn {mso-style-name:"Ingen mellomrom Tegn"; mso-style-priority:1; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:"Ingen mellomrom"; mso-ansi-font-size:11.0pt; mso-bidi-font-size:11.0pt; font-family:"Times New Roman",serif; mso-fareast-font-family:"Times New Roman"; mso-fareast-theme-font:minor-fareast; mso-font-kerning:0pt; mso-ligatures:none; mso-fareast-language:NO-BOK;} span.HTML-forhndsformatertTegn {mso-style-name:"HTML-forh�ndsformatert Tegn"; mso-style-noshow:yes; mso-style-priority:99; mso-style-unhide:no; mso-style-locked:yes; mso-style-link:HTML-forh�ndsformatert; mso-ansi-font-size:10.0pt; mso-bidi-font-size:10.0pt; font-family:Consolas; mso-ascii-font-family:Consolas; mso-hansi-font-family:Consolas;} span.msoIns {mso-style-type:export-only; mso-style-name:""; text-decoration:underline; text-underline:single; color:teal;} span.msoDel {mso-style-type:export-only; mso-style-name:""; text-decoration:line-through; color:red;} span.SpellE {mso-style-name:""; mso-spl-e:yes;} span.GramE {mso-style-name:""; mso-gram-e:yes;} .MsoChpDefault {mso-style-type:export-only; mso-default-props:yes; font-size:12.0pt; mso-ansi-font-size:12.0pt; mso-bidi-font-size:12.0pt; font-family:"Aptos",sans-serif; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi; mso-fareast-language:EN-US;} .MsoPapDefault {mso-style-type:export-only; margin-bottom:8.0pt; line-height:115%;} /\* Page Definitions \*/ @page {mso-footnote-separator:url("media-filer/header.htm") fs; mso-footnote-continuation-separator:url("media-filer/header.htm") fcs; mso-endnote-separator:url("media-filer/header.htm") es; mso-endnote-continuation-separator:url("media-filer/header.htm") ecs;} @page WordSection1 {size:595.3pt 841.9pt; margin:70.85pt 70.85pt 70.85pt 70.85pt; mso-header-margin:35.4pt; mso-footer-margin:35.4pt; mso-page-numbers:0; mso-title-page:yes; mso-footer:url("media-filer/header.htm") f1; mso-paper-source:0;} div.WordSection1 {page:WordSection1;} /\* List Definitions \*/ @list l0 {mso-list-id:96098861; mso-list-type:hybrid; mso-list-template-ids:-1615574848 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l0:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l0:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l0:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l0:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l1 {mso-list-id:153881823; mso-list-type:hybrid; mso-list-template-ids:-1289564718 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l1:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l1:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l1:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l1:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l2 {mso-list-id:168371002; mso-list-type:hybrid; mso-list-template-ids:704141794 -1867734470 68419587 68419589 68419585 68419587 68419589 68419585 68419587 68419589;} @list l2:level1 {mso-level-start-at:0; mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi;} @list l2:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l2:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} @list l2:level4 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol;} @list l2:level5 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l2:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} @list l2:level7 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol;} @list l2:level8 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l2:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} @list l3 {mso-list-id:248346248; mso-list-type:hybrid; mso-list-template-ids:1626352568 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l3:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l3:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l3:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l3:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l4 {mso-list-id:284966715; mso-list-template-ids:674542158;} @list l4:level1 {mso-level-start-at:3; mso-level-text:%1; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:18.0pt; text-indent:-18.0pt;} @list l4:level2 {mso-level-number-format:roman-upper; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:54.0pt; text-indent:-18.0pt; mso-ascii-font-family:Aptos; mso-ascii-theme-font:minor-latin; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-hansi-font-family:Aptos; mso-hansi-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi;} @list l4:level3 {mso-level-text:"%1\\.%2\\.%3"; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-36.0pt;} @list l4:level4 {mso-level-text:"%1\\.%2\\.%3\\.%4"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:162.0pt; text-indent:-54.0pt;} @list l4:level5 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:198.0pt; text-indent:-54.0pt;} @list l4:level6 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:252.0pt; text-indent:-72.0pt;} @list l4:level7 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:288.0pt; text-indent:-72.0pt;} @list l4:level8 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7\\.%8"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:342.0pt; text-indent:-90.0pt;} @list l4:level9 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7\\.%8\\.%9"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:378.0pt; text-indent:-90.0pt;} @list l5 {mso-list-id:384526537; mso-list-type:hybrid; mso-list-template-ids:1404489720 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l5:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l5:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l5:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l5:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l6 {mso-list-id:386300931; mso-list-type:hybrid; mso-list-template-ids:2066525470 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l6:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l6:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l6:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l6:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l7 {mso-list-id:402606121; mso-list-type:hybrid; mso-list-template-ids:-875381172 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l7:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l7:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l7:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l7:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l8 {mso-list-id:716778951; mso-list-type:hybrid; mso-list-template-ids:1455844798 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l8:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l8:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l8:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l8:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l9 {mso-list-id:821042837; mso-list-type:hybrid; mso-list-template-ids:2105313232 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l9:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l9:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l9:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l9:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l10 {mso-list-id:828592053; mso-list-type:hybrid; mso-list-template-ids:-189993872 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l10:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l10:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l10:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l10:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l11 {mso-list-id:901141752; mso-list-type:hybrid; mso-list-template-ids:1102081142 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l11:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l11:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l11:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l11:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l12 {mso-list-id:931936207; mso-list-type:hybrid; mso-list-template-ids:-434881030 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l12:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l12:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l12:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l12:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l13 {mso-list-id:1096515099; mso-list-template-ids:1480595664;} @list l13:level1 {mso-level-number-format:none; mso-level-text:"1\\."; mso-level-tab-stop:36.0pt; mso-level-number-position:left; margin-left:1.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt;} @list l13:level2 {mso-level-start-at:4; mso-level-tab-stop:39.4pt; mso-level-number-position:left; margin-left:31.75pt; text-indent:-10.5pt;} @list l13:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:92.7pt; mso-level-number-position:left; margin-left:3.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:121.05pt; mso-level-number-position:left; margin-left:4.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:149.4pt; mso-level-number-position:left; margin-left:5.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:177.75pt; mso-level-number-position:left; margin-left:6.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:206.1pt; mso-level-number-position:left; margin-left:7.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:234.45pt; mso-level-number-position:left; margin-left:8.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l13:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:262.8pt; mso-level-number-position:left; margin-left:9.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l14 {mso-list-id:1269579845; mso-list-type:hybrid; mso-list-template-ids:-312324558 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l14:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l14:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l14:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l14:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l15 {mso-list-id:1271817487; mso-list-type:hybrid; mso-list-template-ids:-1638485336 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l15:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l15:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l15:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l15:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l16 {mso-list-id:1292632968; mso-list-type:hybrid; mso-list-template-ids:1432495890 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l16:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l16:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l16:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l16:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l17 {mso-list-id:1328244956; mso-list-type:hybrid; mso-list-template-ids:394720220 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l17:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l17:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l17:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l17:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l18 {mso-list-id:1350643818; mso-list-type:hybrid; mso-list-template-ids:-727917730 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l18:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l18:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l18:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l18:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l19 {mso-list-id:1375618994; mso-list-template-ids:1244701908;} @list l19:level1 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:36.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Symbol;} @list l19:level2 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l19:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:126.0pt; text-indent:-36.0pt;} @list l19:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:144.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l19:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:180.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l19:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:216.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l19:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:252.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l19:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:288.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l19:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:324.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l20 {mso-list-id:1392272175; mso-list-type:hybrid; mso-list-template-ids:1431486294 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l20:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l20:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l20:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l20:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l21 {mso-list-id:1404445641; mso-list-type:hybrid; mso-list-template-ids:-1522081054 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l21:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l21:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l21:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l21:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l22 {mso-list-id:1410422785; mso-list-type:hybrid; mso-list-template-ids:-247172046 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l22:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l22:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l22:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l22:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l23 {mso-list-id:1452355879; mso-list-type:hybrid; mso-list-template-ids:1534229626 2089206468 68419587 68419589 68419585 68419587 68419589 68419585 68419587 68419589;} @list l23:level1 {mso-level-number-format:bullet; mso-level-text:-; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:54.0pt; text-indent:-18.0pt; font-family:"Courier New"; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin;} @list l23:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:90.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l23:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:126.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l23:level4 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:162.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l23:level5 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:198.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l23:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:234.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l23:level7 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:270.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l23:level8 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:306.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l23:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:342.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l24 {mso-list-id:1566797155; mso-list-type:hybrid; mso-list-template-ids:-1816330708 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l24:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l24:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l24:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l24:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l25 {mso-list-id:1581259069; mso-list-type:hybrid; mso-list-template-ids:-1381619894 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l25:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l25:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l25:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l25:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l26 {mso-list-id:1599022104; mso-list-type:hybrid; mso-list-template-ids:-2135626906 -686649840 68419587 68419589 68419585 68419587 68419589 68419585 68419587 68419589;} @list l26:level1 {mso-level-start-at:8; mso-level-number-format:bullet; mso-level-text:-; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:54.0pt; text-indent:-18.0pt; font-family:"Aptos",sans-serif; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi;} @list l26:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:90.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l26:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:126.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l26:level4 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:162.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l26:level5 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:198.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l26:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:234.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l26:level7 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:270.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l26:level8 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:306.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l26:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:342.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l27 {mso-list-id:1638609809; mso-list-template-ids:-1368122710;} @list l27:level1 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:36.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Symbol;} @list l27:level2 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l27:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:108.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:144.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:180.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:216.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:252.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:288.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l27:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:324.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l28 {mso-list-id:1689989360; mso-list-type:hybrid; mso-list-template-ids:693435456 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l28:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l28:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l28:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l28:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l29 {mso-list-id:1716615955; mso-list-template-ids:1480595664;} @list l29:level1 {mso-level-number-format:none; mso-level-text:"1\\."; mso-level-tab-stop:36.0pt; mso-level-number-position:left; margin-left:1.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt;} @list l29:level2 {mso-level-start-at:4; mso-level-tab-stop:39.4pt; mso-level-number-position:left; margin-left:31.75pt; text-indent:-10.5pt;} @list l29:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:92.7pt; mso-level-number-position:left; margin-left:3.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:121.05pt; mso-level-number-position:left; margin-left:4.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:149.4pt; mso-level-number-position:left; margin-left:5.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:177.75pt; mso-level-number-position:left; margin-left:6.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:206.1pt; mso-level-number-position:left; margin-left:7.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:234.45pt; mso-level-number-position:left; margin-left:8.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l29:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:262.8pt; mso-level-number-position:left; margin-left:9.0cm; text-indent:-10.5pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l30 {mso-list-id:1736931548; mso-list-type:hybrid; mso-list-template-ids:-6267650 -1 -1 -1 -1 -1 -1 -1 -1 -1;} @list l30:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l30:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l30:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l30:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l31 {mso-list-id:1750078961; mso-list-type:hybrid; mso-list-template-ids:-6267650 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l31:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l31:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l31:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l31:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l32 {mso-list-id:1761218965; mso-list-type:hybrid; mso-list-template-ids:982428870 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l32:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l32:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l32:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l32:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l33 {mso-list-id:1797215162; mso-list-type:hybrid; mso-list-template-ids:-760827202 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l33:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l33:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l33:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l33:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l34 {mso-list-id:1848594850; mso-list-type:hybrid; mso-list-template-ids:-1710465566 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l34:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l34:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l34:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l34:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l35 {mso-list-id:1881045813; mso-list-type:hybrid; mso-list-template-ids:1654562626 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l35:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l35:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l35:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l35:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l36 {mso-list-id:1951161755; mso-list-template-ids:-1051443502;} @list l36:level1 {mso-level-start-at:3; mso-level-text:%1; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:18.0pt; text-indent:-18.0pt;} @list l36:level2 {mso-level-start-at:5; mso-level-text:"%1\\.%2"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:36.0pt; text-indent:-18.0pt;} @list l36:level3 {mso-level-text:"%1\\.%2\\.%3"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:72.0pt; text-indent:-36.0pt;} @list l36:level4 {mso-level-text:"%1\\.%2\\.%3\\.%4"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:108.0pt; text-indent:-54.0pt;} @list l36:level5 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:126.0pt; text-indent:-54.0pt;} @list l36:level6 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:162.0pt; text-indent:-72.0pt;} @list l36:level7 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:180.0pt; text-indent:-72.0pt;} @list l36:level8 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7\\.%8"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:216.0pt; text-indent:-90.0pt;} @list l36:level9 {mso-level-text:"%1\\.%2\\.%3\\.%4\\.%5\\.%6\\.%7\\.%8\\.%9"; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:234.0pt; text-indent:-90.0pt;} @list l37 {mso-list-id:1967735612; mso-list-type:hybrid; mso-list-template-ids:1432495890 -1 -1 -1 -1 -1 -1 -1 -1 -1;} @list l37:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l37:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l37:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l37:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l38 {mso-list-id:1980301340; mso-list-type:hybrid; mso-list-template-ids:-127861254 68419599 68419609 68419611 68419599 68419609 68419611 68419599 68419609 68419611;} @list l38:level1 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level2 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level3 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l38:level4 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level5 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level6 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l38:level7 {mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level8 {mso-level-number-format:alpha-lower; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt;} @list l38:level9 {mso-level-number-format:roman-lower; mso-level-tab-stop:none; mso-level-number-position:right; text-indent:-9.0pt;} @list l39 {mso-list-id:1984581463; mso-list-template-ids:278314858;} @list l39:level1 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:36.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Symbol;} @list l39:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:72.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:"Courier New"; mso-bidi-font-family:"Times New Roman";} @list l39:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:108.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:144.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:180.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:216.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:252.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:288.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l39:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:324.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l40 {mso-list-id:1993021989; mso-list-type:hybrid; mso-list-template-ids:-1637169288 -2087665756 68419587 68419589 68419585 68419587 68419589 68419585 68419587 68419589;} @list l40:level1 {mso-level-number-format:bullet; mso-level-text:-; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:54.0pt; text-indent:-18.0pt; font-family:"Aptos",sans-serif; mso-fareast-font-family:Aptos; mso-fareast-theme-font:minor-latin; mso-bidi-font-family:"Times New Roman"; mso-bidi-theme-font:minor-bidi;} @list l40:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:90.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l40:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:126.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l40:level4 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:162.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l40:level5 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:198.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l40:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:234.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l40:level7 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:270.0pt; text-indent:-18.0pt; font-family:Symbol;} @list l40:level8 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:306.0pt; text-indent:-18.0pt; font-family:"Courier New";} @list l40:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; margin-left:342.0pt; text-indent:-18.0pt; font-family:Wingdings;} @list l41 {mso-list-id:2056925873; mso-list-template-ids:-509052066;} @list l41:level1 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:36.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Symbol;} @list l41:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:72.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:"Courier New"; mso-bidi-font-family:"Times New Roman";} @list l41:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:108.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level4 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:144.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level5 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:180.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:216.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level7 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:252.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level8 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:288.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l41:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:324.0pt; mso-level-number-position:left; text-indent:-18.0pt; mso-ansi-font-size:10.0pt; font-family:Wingdings;} @list l42 {mso-list-id:2102220513; mso-list-type:hybrid; mso-list-template-ids:1921054020 68419585 68419587 68419589 68419585 68419587 68419589 68419585 68419587 68419589;} @list l42:level1 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol;} @list l42:level2 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l42:level3 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} @list l42:level4 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol;} @list l42:level5 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l42:level6 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} @list l42:level7 {mso-level-number-format:bullet; mso-level-text:\\F0B7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Symbol;} @list l42:level8 {mso-level-number-format:bullet; mso-level-text:o; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:"Courier New";} @list l42:level9 {mso-level-number-format:bullet; mso-level-text:\\F0A7; mso-level-tab-stop:none; mso-level-number-position:left; text-indent:-18.0pt; font-family:Wingdings;} ol {margin-bottom:0cm;} ul {margin-bottom:0cm;} -->

Table of Contents

[Before we begin.. 5](#_Toc182987699)

[Info about TL;DR. 5](#_Toc182987700)

[Legal Disclaimer. 5](#_Toc182987701)

[Introduction.. 5](#_Toc182987702)

[What are the \*arrs?. 7](#_Toc182987703)

[From the wiki itself: 7](#_Toc182987704)

[In Simple terms: 7](#_Toc182987705)

[Prowlarr: 7](#_Toc182987706)

[Radarr. 7](#_Toc182987707)

[Sonarr. 7](#_Toc182987708)

[Lidarr. 7](#_Toc182987709)

[Readarr. 7](#_Toc182987710)

[Whisparr. 8](#_Toc182987711)

[Bazarr. 8](#_Toc182987712)

[Flaresolverr. 8](#_Toc182987713)

[Overseerr. 8](#_Toc182987714)

[Requestrr. 8](#_Toc182987715)

[Arr-stack: 8](#_Toc182987716)

[All the different \*arr apps (and related ones that I know of) 9](#_Toc182987717)

[The apps I will cover in this guide. 11](#_Toc182987718)

[Hardware specs. 12](#_Toc182987719)

[Minimum requirements. 12](#_Toc182987720)

[CPU.. 12](#_Toc182987721)

[RAM.. 12](#_Toc182987722)

[Storage. 12](#_Toc182987723)

[Recommended requirements. 13](#_Toc182987724)

[CPU.. 13](#_Toc182987725)

[RAM.. 13](#_Toc182987726)

[Storage. 13](#_Toc182987727)

[Recommended NAS models for this setup. 14](#_Toc182987728)

[Minimum.. 14](#_Toc182987729)

[Recommended. 14](#_Toc182987730)

[Models to avoid. 15](#_Toc182987731)

[Low-End ARM-Based NAS Models. 15](#_Toc182987732)

[Why not: 15](#_Toc182987733)

[Models with Less Than 2 GB RAM.. 15](#_Toc182987734)

[Why not: 15](#_Toc182987735)

[Older/Legacy Models. 16](#_Toc182987736)

[Why not: 16](#_Toc182987737)

[Single-Bay NAS Models. 16](#_Toc182987738)

[Why not: 16](#_Toc182987739)

[Models without integrated graphics. 16](#_Toc182987740)

[Why not: 16](#_Toc182987741)

[What you need instead.. 17](#_Toc182987742)

[TL;DR. 18](#_Toc182987743)

[Preparations. 24](#_Toc182987744)

[Folder Structure. 24](#_Toc182987745)

[The folder structure should look like this: 25](#_Toc182987746)

[Media. 25](#_Toc182987747)

[Docker. 26](#_Toc182987748)

[Setting permissions. 27](#_Toc182987749)

[The installation.. 28](#_Toc182987750)

[Setting up the start up script for glueTUN.. 28](#_Toc182987751)

[Firewall rules (if you have firewall set up) 31](#_Toc182987752)

[WireGuard Kernel Module. 34](#_Toc182987753)

[Creating a Synology bridge network. 36](#_Toc182987754)

[Docker project. 37](#_Toc182987755)

[Required. 37](#_Toc182987756)

[GlueTUN: 38](#_Toc182987757)

[Ports. 39](#_Toc182987758)

[Volumes. 39](#_Toc182987759)

[Environment. 39](#_Toc182987760)

[VPN Service provider. 39](#_Toc182987761)

[Proxy. 45](#_Toc182987762)

[Timezone. 45](#_Toc182987763)

[Firewall Outbound Subnets. 45](#_Toc182987764)

[Network\_mode. 46](#_Toc182987765)

[labels: 46](#_Toc182987766)

[\- com.centurylinklabs.watchtower.enable=false. 46](#_Toc182987767)

[security\_opt: 46](#_Toc182987768)

[\- no-new-privileges:true: 46](#_Toc182987769)

[Restart: always. 46](#_Toc182987770)

[Full GlueTUN docker-compose.yml 46](#_Toc182987771)

[Download client 48](#_Toc182987772)

[network\_mode. 48](#_Toc182987773)

[Environment. 48](#_Toc182987774)

[PUID and PGID.. 48](#_Toc182987775)

[UMASK.. 49](#_Toc182987776)

[Volumes. 49](#_Toc182987777)

[Full docker-compose.yml for qbittorrent. 50](#_Toc182987778)

[Sonarr 51](#_Toc182987779)

[Something important: 51](#_Toc182987780)

[Full docker-compose.yml file. 52](#_Toc182987781)

[Radarr 53](#_Toc182987782)

[Lidarr 54](#_Toc182987783)

[Prowlarr 55](#_Toc182987784)

[Flaresolverr 56](#_Toc182987785)

[Overseerr 57](#_Toc182987786)

[Requestrr 58](#_Toc182987787)

[Tautulli 59](#_Toc182987788)

[Putting it all together 60](#_Toc182987789)

[Common Errors. 65](#_Toc182987790)

[Configuration of the apps. 67](#_Toc182987791)

[qBitTorrent. 67](#_Toc182987792)

[Login. 67](#_Toc182987793)

[Change username and password. 68](#_Toc182987794)

[Change downloads path. 69](#_Toc182987795)

[Radarr. 70](#_Toc182987796)

[Adding Authentication method. 70](#_Toc182987797)

[Adding Root Folder 71](#_Toc182987798)

[Changing Movie Naming Scheme. 72](#_Toc182987799)

[Quality Settings (File Size) 74](#_Toc182987800)

[Quality profiles. 75](#_Toc182987801)

[Sonarr. 76](#_Toc182987802)

[Adding Root Folder(s) 76](#_Toc182987803)

[Changing Naming Scheme(s) 78](#_Toc182987804)

[Quality Settings (File Size) 79](#_Toc182987805)

[Quality Profiles. 80](#_Toc182987806)

[Quality Profiles (Anime) 81](#_Toc182987807)

[Lidarr. 82](#_Toc182987808)

[Adding Root Folder(s) 82](#_Toc182987809)

[Quality Settings. 84](#_Toc182987810)

[Connecting download client to Radarr, Sonarr and Lidarr. 85](#_Toc182987811)

[Prowlarr. 88](#_Toc182987812)

[Adding the apps to Prowlarr 88](#_Toc182987813)

[How do I get the API key?. 91](#_Toc182987814)

[Connecting Flaresolverr 92](#_Toc182987815)

[Adding indexers. 94](#_Toc182987816)

[Overseerr. 97](#_Toc182987817)

[Configuring Overseerr 97](#_Toc182987818)

[Adding Radarr and Sonarr 99](#_Toc182987819)

[Radarr. 100](#_Toc182987820)

[Sonarr. 102](#_Toc182987821)

[Requestrr 105](#_Toc182987822)

[Configuring Requestrr. 105](#_Toc182987823)

[How to get Discord Application Id and Bot Token.. 105](#_Toc182987824)

[How to invite the bot to our Discord server. 110](#_Toc182987825)

[Connecting Requestrr to Overseerr (Or Radarr, Sonarr, Ombi). 111](#_Toc182987826)

[Modifications to set it up for UseNet. 113](#_Toc182987827)

[FAQ.. 113](#_Toc182987828)

[What is Usenet?. 113](#_Toc182987829)

[What is UseNet used for 113](#_Toc182987830)

[Why are the files split into parts?. 113](#_Toc182987831)

[Do I need to manually combine all the parts of the files afterwards?. 113](#_Toc182987832)

[UseNet vs Torrenting for Media Downloads. 113](#_Toc182987833)

[Why are people talking about Linux ISOs?. 114](#_Toc182987834)

[What is the difference between providers and idnexers, and what are their roles?. 114](#_Toc182987835)

[A lot of the provider deals, especially on black Friday, is for 15 months instead of 12. Is this a trick to make you renew when it�s not a sale?. 115](#_Toc182987836)

[Pros and Cons list for Torrent vs UseNet. 116](#_Toc182987837)

[Okay, I�m convinced. But what provider should I go for, and should I do an unlimited monthly/yearly plan or a block account?. 117](#_Toc182987838)

[Okay cool, what about indexer?. 117](#_Toc182987839)

[Wow, that�s a lot of choices. What do you recommend for a beginner?. 119](#_Toc182987840)

[What is a newsreader?. 120](#_Toc182987841)

[Now I have a provider and an indexer, how to set it up with the \*arrs?. 121](#_Toc182987842)

[Configuring the apps. 123](#_Toc182987843)

[Sabmzbd. 123](#_Toc182987844)

[NZBHydra2. 124](#_Toc182987845)

[Sources. 128](#_Toc182987846)   

Before we begin
===============

If you find any mistakes, incorrect facts, or would like to give your feedback, you can go so either by contacting me on Reddit, Discord or Github.

Reddit: [https://www.reddit.com/user/MattiTheGamer/](https://www.reddit.com/user/MattiTheGamer/)

Discord: @matti1003

Github: [https://github.com/MathiasFurenes/synology-arr-guide/tree/main](https://github.com/MathiasFurenes/synology-arr-guide/tree/main)

If you want to you can also support me with a PayPal donation here:

[https://www.paypal.com/donate/?hosted\_button\_id=DK7VP9RD2LEQ2](https://www.paypal.com/donate/?hosted_button_id=DK7VP9RD2LEQ2)

Info about TL;DR
----------------

The [TL;DR](#_TL;DR) comes before the main guide. For the best experience, skip this section and go to the [full guide](#_Preparations). The [TL;DR](#_TL;DR) only covers the installation, and NOT the [configs](#Configs) as they are too complex to put in a TL;DR. It also requires some knowledge on docker beforehand so you can edit the docker-compose to match your system. I have also not added anything UseNet related to the TL;DR.

Legal Disclaimer
----------------

For legal reasons I must state that I do not condone illegal pirating of copyrighted material. This is made for educational purposes only. I expect that everyone who follows this guide will only use this for legal purposes, like downloading free to use Linux ISOs. Please never ever use this to illegally download copyrighted material such as, but not limited to, movies and TV Shows.

Introduction
------------

Before we start let�s figure out your needs. Do you want to download movies, tv shows, music, e-books, comics or adult videos? Most likely you want a combination of a lot of them. We also need to figure out whether you want it to be connected to a VPN. Here is a break-down of all the apps and their use-cases:

  

What are the \*arrs?
--------------------

### From the wiki itself:

�Lidarr, Prowlarr, Radarr, Readarr, Sonarr, and Whisparr are collectively referred to as "\*arr" or "\*arrs". They are designed to automatically grab, sort, organize, and monitor your Music, Movie, E-Book, or TV Show collections for Lidarr, Radarr, Readarr, Sonarr, and Whisparr; and to manage your indexers and keep them in sync with the aforementioned apps for Prowlarr.�

### In Simple terms:

#### Prowlarr:

An index manager. This just means it searches for files to download on websites you assign it.

Radarr:

When Prowlarr find a movie file, it gives it to Radarr. Radarr then send it over to a download client, like QBitTorrent. After it�s done downloading, Radarr takes it away from QBItTorrent again and rename the file appropriately before it puts it inside your Media library.

Sonarr:

Same as Radarr, but for TV shows.

Lidarr:

Same as Radarr, but for music

Readarr:

Same as Radarr, but for e-books

Whisparr:

Same as Radarr, but for adult videos

Bazarr:

Connects with Radarr and Sonarr to download subtitles for your movies and TV shows.

Flaresolverr:

Bypasses cloudfare solver

Overseerr**:**

�A requesting application where you browse or search for movies and TV shows, kinda like Netflix, and with a� click of a button they start downloading to your own media collection!

Requestrr**:**

Goes together with Overseerr or Radarr and Sonarr to allow for requesting through discord chat.

#### Arr\-stack:

The arr\-stack just refers to a collection of these applications bundled and working together.  

All the different \*arr apps (and related ones that I know of)
--------------------------------------------------------------

**Prowlarr** � Index manager. It searches the torrent sites for downloads (Recommended for everyone)

**Flaresolverr** � Some indexers require you to solve a Cloudflare captcha. Flaresolverr can do this.

**Jackett** � Alternative to Prowlarr. Most find Prowlarr to be both easier to set up and better to use.

**Sonarr** � TV Shows/Anime Shows downloader.

**Radarr** � Movie downloader.

**Lidarr** � Music downloader.

**Readarr** � E-book downloader

**Mylar** � Comics downloader.

**Bazarr** � Subtitle downloader for your Movies and TV Shows.

**Lazy Librarian** � A program to follow authors and grab metadata for digital reading.

**Whisparr** � Adult videos downloader.

**GlueTUN** � Required for use of VPN

**Plex** � A frontend to your media server. It�s where you access all your media, in the style of something like Netflix. It also has a very good Spotify-like app called plexamp.

**Jellyfin** � Also a frontend to your media server. Jellyfin is, in contrast to Plex, open-source. This means that all of it�s features is and always will be free, but it also means that it doesn�t have the same funding and therefore might not have all of the features Plex has.

**Overseerr** � Allows for easy requesting of movies and TV shows to add to Plex.

**Jellyseerr** � Same as Overseer but for Jellyfin.

**Ombi** � App to request Movies and TV Shows for plex or Emby.

**Requestrr** � Allows for requests for Sonarr and Radarr via chat, like Discord. It can also be integrated with Ombi and Overseer.

**qBitTorrent** � Torrent download client.

**NZBGet** � NZB download client.

**Tautulli** � Plex media server statistics

There are even more, but I have not gotten into these myself. These are the ones I have atleast some knowledge about.

  

The apps I will cover in this guide
-----------------------------------

I would like to cover as many as possible, but I have not used or tried some of them myself. I host on Plex, so I use Overseer, and have not tried neither Jellyseer or Ombi. Even though I�m pretty sure Jellyseer is the exact same just for Jellyfin. But you should always read the official docs yourself. Anyway, the apps I will go over is:

�         GlueTUN

�         Prowlarr

�         Flaresolverr

�         Sonarr

�         Radarr

�         Lidarr

�         Overseer

�         Requestrr

�         qBitTorrent

�         Tautulli

�         Sabznbd (UseNet)

�         NZBHydra2 (UseNet)

  

Hardware specs
--------------

I am running all this on a DS423+, with an extra 16GB memory stick and 512GB SSD cache. I have not tested it myself on any other devices, but I have made a few google searches and asked ChatGPT for some help to determine the systems requirements. Therefore, I ask you to take these number with a grain of salt.

### Minimum requirements

#### CPU

A quad-core 64bit CPU with x86 architecture. (Docker can only run on x86, and not any ARM CPUs natively. You might be able to still try this out, but you will have to do some workarounds.) An Intel Celeron J4105 or Intel Celeron J4125 should be sufficient for basic use.

#### RAM

4GB RAM (reported by ChatGPT). I think it might be able to run on 2GB for low, basic use. But don�t expect the best performance

#### Storage

These apps don�t take up more than 2GB-5GB for database and configs.

A 2-hour movie in 480p will take 700MB-2GB space, and 3GB-6GB in 720p. A 12-episode TV show with 45 minutes long episodes will take 4GB-10GB in 480p and 12GB-27GB in 720p

  

### Recommended requirements

#### CPU

Intel Celeron J4125 or higher. For best performance, Intel Core i3/i5 or AMD equivalent. But since most will probably run this on a Synology, the J4125 or better is sufficient.

#### RAM

8GB RAM. For best performance, an upgrade to 16GB will make it a lot smoother.

#### Storage

A 2-hour long movie in 1080p will take 8GB-15GB storage space, and in 4k it will be about 20GB-50GB. A 12-episode show with 45 minutes long episodes will take up 35GB-60GB in 1080p and 90GB-225GB in 4k.

  

Recommended NAS models for this setup
-------------------------------------

Since I assume most people will use a Synology NAS, as this is what this guide was meant for, I will list some recommendations.

### Minimum

�         **Synology DS220+**

\-          CPU: Intel Celeron J4025 (dual-core)

\-          RAM: 2GB (expandable to 6GB)

\-          Suitable for running a few applications simultaneously with small to medium libraries.

�         **Synology DS720+**

\-          CPU: Intel Celeron J4125 (quad-core)

\-          RAM: 2GB (expandable to 6GB)

\-          Great for small to mid-size media libraries, running Docker containers, and handling multiple tasks at once.

### Recommended

�         **Synology DS920+**

\-          CPU: Intel Celeron J4125 (quad-core)

\-          RAM: 4GB (expandable to 8GB)

\-          Supports SSD caching, making it a solid choice for heavier workloads like streaming, transcoding, and multiple apps running concurrently.

�         **Synology DS423+**

\-          CPU: Intel Celeron J4125 (quad-core)

\-          2GB RAM (Recommended to upgrade to at least 4GB or 6GB)

\-          4-bay NAS with support for 2 NVME drives

�         **Synology DS1821+**

\-          CPU: AMD Ryzen V1500B (quad-core)

\-          RAM: 4GB (expandable to 32GB)

\-          8-bay NAS with strong processing power for large libraries and heavy multitasking.

  

### Models to avoid

#### Low-End ARM-Based NAS Models

�         **Synology DS216j� (**Marvell Armada 385, dual-core 1.0GHz, 512MB)

�         **Synology DS218j** (Marvell Armada 385, Dual-Core 1.3 GHz, 512 MB RAM)

�         **Synology DS219j** (Marvell Armada 3720, Dual-core 800 MHz, 256 MB RAM)

�         **Synology DS220j** (Realtek RTD1296, Quad-Core 1.4 GHz, 512 MB RAM)

##### Why not:

1.  **CPU**: These models come with weak, low-power ARM processors that are not suited for running multiple Docker containers or handling tasks like torrenting and media management.

1.  **RAM**: Most of these devices have **512 MB RAM or less**, which is far too little for running multiple services in Docker.

1.  **Docker Support**: ARM-based models may not fully support Docker, especially for complex workloads, and will struggle with performance under even light to moderate use.

#### Models with Less Than 2 GB RAM

1.  **Synology DS220j** (512 MB RAM)

1.  **Synology DS218play** (1 GB RAM)

1.  **Synology DS218** (2 GB RAM)

1.  **Synology DS118** (1 GB RAM)

##### Why not:

*   **Insufficient RAM**: Apps like **Overseerr** and **qBittorrent** require more memory, and these models would quickly run out of resources. With less than 2 GB, you'll experience poor performance, constant swapping to disk, or the inability to run all your containers simultaneously.
*   **No Upgrade Path**: Many of these models do not allow you to upgrade the RAM, so you're stuck with what they offer.

#### Older/Legacy Models

�         **Synology DS214+** (Dual-core 1.33 GHz, 1 GB RAM)

�         **Synology DS415play** (Intel Atom CE5335, Dual-core 1.6 GHz, 1 GB RAM)

�         **Synology DS216play** (ARM Cortex-A9, Dual-core 1.5 GHz, 1 GB RAM)

##### Why not:

*   **Outdated CPU architecture**: These older CPUs lack the power and modern architecture needed for virtualization and handling Docker workloads.
*   **RAM limitations**: Even if some of these have x86 architecture, 1 GB or even 2 GB of RAM is not sufficient for your use case.

#### Single-Bay NAS Models

�         **Synology DS118** (Realtek RTD1296, Quad-core 1.4 GHz, 1 GB RAM)

�         **Synology DS119j** (Marvell Armada 3700, Dual-core 800 MHz, 256 MB RAM)

##### Why not:

*   **Low performance**: These single-bay models come with very basic hardware, meaning you�ll struggle to run Docker and multiple applications.
*   **No redundancy**: With only one drive, there�s no data redundancy (no RAID), which is a concern when managing large amounts of media files.

#### Models without integrated graphics

�         Synology DS923+ (AMD Ryzen R1600, Quad-core 2.6GHz, 4GB RAM)

�         Synology DS 1522+ (AMD Ryzen R1600, Quad-core 2.6GHz, 8GB RAM)

##### Why not:

*   **No integrated graphics**: Although these can work just fine, they are not ideal as you won�t be able to do hardware transcoding. For native playback of h264 files these can be perfect.

#### What you need instead

To run this full arr\-stack smoothly on Docker, aim for:

*   **x86-64 architecture** (with embedded graphics)
*   **Minimum 4 GB RAM**, ideally **8 GB or more**.
*   **Expandable RAM** for future growth.
*   **At least dual-bay** for RAID redundancy.

TL;DR
=====

If you don�t want to read all that, just do this:

1.      Create these folder inside /volume1/docker/arr\-stack:

�         gluetun

�         lidarr > config

�         overseer > config

�         prowlarr > config

�         qbittorrent > config, downloads

�         radarr >config

�         requestrr > config

�         sonar > config

2.      SSH into your NAS and type these commands

\-   sudo chmod -R 777 /volume1/Media

\-   id. Take note of the GID and UID output

\-   sudo chown -R < UID>:< GID> \\volume1\\Media

3.      Go to Task Scheduler and create a trigger task on start-up to run this script:

#!/bin/sh -e

insmod /lib/modules/tun.ko

I.        Create a firewall rule to allow port 1194 and 1195

II.      Go to think link: [https://www.blackvoid.club/wireguard-spk-for-your-synology-nas/](https://www.blackvoid.club/wireguard-spk-for-your-synology-nas/). Find the correct version for your system and manually install the .spk file in package cener. Don�t run when finished. Reboot afterwards

III.    SSH into your device and type this command:

IV.   /var/packages/WireGuard/scripts/start

4. �Find out how to configure GlueTUN for your VPN provider:

[https://github.com/qdm12/gluetun-wiki/tree/main/setup/providers](https://github.com/qdm12/gluetun-wiki/tree/main/setup/providers)

5. Create a new network inside container manager. Configure the network like this:

\-          Subnet: 172.20.0.0/16

\-          IP range: 172.20.0.2/25

\-          Gateway: 172.20.0.1

\-          IPv6: Disabled

\-          IP Masquerade: enabled (Leave the �disable� option unticked)

6\. Create a new docker project. Path should be /volume1/docker/arr\-stack. Paste this docker-compose.yml wand make any necessary changes:

version: "3"

services:

  gluetun:

    image: qmcgaw/gluetun

    container\_name: gluetun

    hostname: gluetun

    cap\_add:

      \- NET\_ADMIN

    devices:

      - /dev/net/tun:/dev/net/tun

    ports:

      - 6881:6881

      - 6881:6881/udp

      \- 8085:8085 \# qbittorrent

      - 8989:8989 \# Sonarr

      - 9696:9696 \# Prowlarr

      - 7878:7878 \# Radarr

      - 8686:8686 #Lidarr

      - 8191:8191 #FlareSolverr

      \- 5055:5055 #Overseerr

      - 4545:4545 #Requestrr

    volumes:

      - /volume1/docker/arr\-stack/gluetun:/gluetun

    environment:

      - VPN\_SERVICE\_PROVIDER=<your-provider>

      - VPN\_TYPE=wireguard

      - VPN\_DISABLE\_IPV6=true

      \# OpenVPN:

      \# - OPENVPN\_USER=

      \# - OPENVPN\_PASSWORD=

      \# Wireguard:

      - WIREGUARD\_PRIVATE\_KEY= <your-private-key>

      - WIREGUARD\_ADDRESSES=<your-address>

      - DNS=<your-dns\>

      - SERVER\_HOSTNAMES=<your-hostnames>

      - SERVER\_CITIES=<your-city>

      \# Timezone for accurate log times

      - TZ=Europe/Oslo

      \# Server list updater

      \# See https://github.com/qdm12/gluetun-wiki/blob/main/setup/servers.md#update-the-vpn-servers-list

      - UPDATER\_PERIOD=24h

      - FIREWALL\_OUTBOUND\_SUBNETS=172.20.0.0/192.168.0.0/24 #change this in line with your subnet see note on guide

    network\_mode: synobridge

    labels:

      - com.centurylinklabs.watchtower.enable\=false #Disables Watchtower

    security\_opt:

      - no-new-privileges:true #For security

  qbittorrent:

    image: lscr.io/linuxserver/qbittorrent

    container\_name: qbittorrent

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      \- TZ=Europe/Oslo

      - WEBUI\_PORT=8085

      - UMASK=022

    volumes:

      - /volume1/docker/arr\-stack/qbittorrent/config:/config

      - /volume1/Media/Torrents:/Media/Torrents

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: unless-stopped

  sonarr:

    image: lscr.io/linuxserver/sonarr:latest

    container\_name: sonarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/sonarr/config:\\config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  prowlarr:

    image: lscr.io/linuxserver/prowlarr:latest

    container\_name: prowlarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/prowlarr/config:/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  radarr:

    image: lscr.io/linuxserver/radarr:latest

    container\_name: radarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/radarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  lidarr:

    image: lscr.io/linuxserver/lidarr:latest

    container\_name: lidarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/lidarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  flaresolverr:

    image: ghcr.io/flaresolverr/flaresolverr:latest

    container\_name: flaresolverr

    network\_mode: "service:gluetun"

    environment:

      - TZ=Europe/Oslo

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: unless-stopped

  overseerr:

    image: sctx/overseerr:latest

    container\_name: overseerr

    network\_mode: "service:gluetun"

    environment:

      - LOG\_LEVEL=debug

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/overseer/config:/app/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  requestrr:

    image: darkalfx/requestrr

    container\_name: requestrr

    network\_mode: "service:gluetun"

    volumes:

    - /volume1/docker/arr\-stack/requestrr/config:/root/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

11.� For config of apps, I can�t really put it in a TL;DR, as it�s way too long and complicated. Chek out the [full guide](#Configs), or find� out yourself on the official docs. The TL;DR is also not updated for UseNet support. Check out UseNet [here](#_Modifications_to_set).

  

Preparations
============

Folder Structure
----------------

I assume you have Installed container manager (docker) on your Synology system already, but if not do that now. Then we need to go into our �docker� shared folder and make some new folder.

### The arr stack

Inside the �docker� shared folder, create a folder and call it something like �arr\-stack�

Inside �arr\-stack�, create these folders:

�         gluetun

�         lidarr

�         overseer

�         prowlarr

�         qbittorrent

�         radarr

�         requestrr

�         sonar

�         tautulli

�         sabnzbd (Optional, for UseNet only. For more info on UseNet, go [here](#_Modifications_to_set))

�         nzbhydra2 (Optional, mainly for UseNet)

If you have any other apps beside these, create a folder for them too as described in the official docs.

Create a folder called �config� inside lidarr, overseer, prowlarr, qbittorrent, radarr, requestrr, sonar, sabnzbd and tautulli.

  

### If you don�t have a Media folder

Create a new shared folder for housing your media. You can call this Data or Media. Within this shared library, you need another folder where you put the actual media. You can call this Media. In �/volume1/Media/Media� you create a folder for movies, tv shows, anime, music and whatever else you would like. Go back to �/volume1/Media� and create a folder called �torrents.� This is where we download our torrent files with qBitTorrent. Inside it create �Incomplete� and �Complete�. If you want to use Usenet, you can create folder called �UseNet� with �Complete� and �Incomplete� inside it.

### The full folder structure should look like this:

#### Media

├── Torrents

│�� ├── Incomplete

│�� └── Complete

├── Usenet

│�� ├── Incomplete

│�� └── Complete

│������ ├── Movies

│������ ├── Music

|������� ├── Anime TV Shows

│������ └── TV Shows

└── Media

��� ├── Movies

��� ├── Music

��� ├── Anime TV Shows

��� └── TV Shows

  

#### docker

└───arr\-stack

��� ├──bazarr

���� │�� └── config

��� ├── gluetun

��� ├── lidarr

���� │�� └── config

��� ├── sabnzbd (Optional)

���� │�� └── config

��� ├── overseer

��� │�� └── config

��� ├── prowlarr

��� │�� └── config

��� ├── qbittorrent

��� │�� └── config

��� ├── radarr

��� │�� └── config

��� ├── requestrr

��� │�� └── config

��� ├── sonarr

��� │�� └── config

��� ├──nzbhydra2

��� │

��� └── tautulli

��� ����└── config

  

Setting permissions
-------------------

To make sure that all the apps have the right permissions to read and write the relevant folder, we need to ssh into the NAS. I prefer PuTTY, but you can use powershell or anything else that you like.

1.      SSH into your NAS

2.      Type the following 2 commands:

\-   sudo chmod -R 777 /volume1/Media/Media

\-   sudo chmod -R 777 /volume1/Media/Torrents

3.      Find your UID and GID

\-   Type: id

4.      You should get an output like this:

![](media-filer/image001.png)

As you can see, we get an output with uid\=XXXX and gid=YYY.

5.      Type the following 2 commands:

\-   sudo chown -R <UID>:<GID> /volume1/Media/Media

\-   sudo chown -R <UID>:<GID> /volume1/Media/Torrents

**NOTE:** If you have your Media library at another location than �/volume1/Media�, then put your path in the 2 relevant commands.

These commands ensure that we have the correct permissions to read and write the files of the directories and their subdirectories.

  

The installation
================

Now that we have our folder structure ready, let�s begin with the actual installation.

Setting up the start-up script for GlueTUN
------------------------------------------

For GlueTUN to start up automatically, we need to create a task on a schedule.

1.      Open up Control Panel, then click on Task Scheduler.

![](media-filer/image003.png)

2.      Next click on Create, Triggered Task then User Defined Script.

![Et bilde som inneholder tekst, Font, skjermbilde, nummer
Automatisk generert beskrivelse](media-filer/image005.png)

3.      Now enter a name for the script. It doesn�t matter what you choose The user **must** be �root� and �Boot-up� for the Event. Don�t click OK yet.

![Et bilde som inneholder tekst, skjermbilde, programvare, nummer
Automatisk generert beskrivelse](media-filer/image006.png)

4.      On the Task Settings tab copy and paste the code below in the �User-Defined script� section. It will look like screenshot

On the Task Settings tab copy and paste the code below in the �User-Defined script� section:

#!/bin/sh -e

insmod /lib/modules/tun.ko

![Et bilde som inneholder tekst, skjermbilde, programvare, Operativsystem
Automatisk generert beskrivelse](media-filer/image007.png)

5.      You can now press OK and agree to the warning message. Next run the script which will enable the TUN device.

![Et bilde som inneholder tekst, skjermbilde, Font, line
Automatisk generert beskrivelse](media-filer/image009.jpg)

  

Firewall rules (if you have firewall set up)
--------------------------------------------

If you have firewall rules set up on your synology to block all outgoing connections, we need to make some exception rules.

Go into Control Panel > Security > Firewall

![](media-filer/image011.jpg)

Click on Edit Rules and then click on �Create�

![Et bilde som inneholder tekst, skjermbilde, programvare, Nettside
Automatisk generert beskrivelse](media-filer/image013.png)

On the �Ports� section, select �Custom�

![Et bilde som inneholder tekst, skjermbilde, programvare, Operativsystem
Automatisk generert beskrivelse](media-filer/image014.png)

On the screen that appears select the Type as �Destination Port� and Protocol as �All�. In this example I am going to open up both 1194 and 1195 as some providers use UDP and some TCP and these are the most commonly used ports.

![](media-filer/image015.png)

Click on OK. Leave the �Source IP� as �All� and �Action� as �Allow�, then �OK� again to apply.

  

WireGuard Kernel Module
-----------------------

The WireGuard kernel module is not necessary, but it does lower the CPU usage a little bit. This in turn allows for better performance and better power efficiency.

�The default Gluetun Wireguard setup uses a �Userspace� implementation of Wireguard which normally should not use much from a CPU resource perspective. However, on Synology it tends to require high CPU utilisation.

(DrFrankenstein�s Tech Stuff)

[BlackVoid.club](https://www.blackvoid.club/) have put together a Kernel Module for Synology which allows Gluetun to use the lower level Kernel to perform Wireguard duties.

1.      Open this link: [https://www.blackvoid.club/wireguard-spk-for-your-synology-nas/](https://www.blackvoid.club/wireguard-spk-for-your-synology-nas/)

2.      Find your model of NAS under the correct DSM version section (If you are following this guide it will be 7.2) and download the pre compiled .spk file

3.      Head into Package Center and click �Manual Install� on the top right and install the .spk file and **untick** the box to run after install

![Free High-Res Red Circle Outline Png | Download Now for Designs](media-filer/image017.png)![Et bilde som inneholder tekst, programvare, Dataikon, skjermbilde
Automatisk generert beskrivelse](media-filer/image019.png)

4.       Reboot

5.      SSH Into your NAS using PuTTY, powershell or any other SSH client and elevate yourself to root by typing �sudo -I� and entering your password

6.      Enter this command and press enter to start up the module

/var/packages/WireGuard/scripts/start

Creating a Synology bridge network
----------------------------------

As default, there is already a bridge network in container manager for Synology. The problem with the default one is that the IPs it assigns are not static, and therefore may change. This is fine for single containers that don�t communicate with each other, but when connecting multiple containers with IPs the IP address needs to always stay the same. To remedy this, we will create our own bridge network.

1.      Open container manager and click on the network tab to the left.

2.      Click �Add� at the top

3.      Configure the network like this:

\-          Subnet: 172.20.0.0/16

\-          IP range: 172.20.0.2/25

\-          Gateway: 172.20.0.1

\-          IPv6: Disabled

\-          IP Masquerade: enabled (Leave the �disable� option unticked)

  

Docker project
--------------

Now we are ready to create the project. A docker project is just a collection of multiple docker containers.

1.      Open �container manager� and head to the �Project� tab.

2.      Click create

3.      Give the project a name. I chose �arr\-stack�

4.      Set the path to be �docker > arr\-stack� (should say �\\docker\\arr\-stack�)

5.      As source, select �Create docker-compose.yml�

Now this next step will be just a little bit different for everyone. What you will put in the docker-compose, will depend on what apps you plan to use and what VPN provider you have. But don�t worry, as you can always come back to the project and edit the docker-compose to add more apps, or to fix any potential problems that may occur. I will try my best to explain what each section does, and if it is relevant to you or not.

### Required

Everyone will need to start the docker-compose out like this:

version: "3"

services:

Then under services we will add all of our apps and configs to each app.

  

### GlueTUN:

  gluetun:

    image: qmcgaw/gluetun

    container\_name: gluetun

    hostname: gluetun

    cap\_add:

      - NET\_ADMIN

    devices:

      \- /dev/net/tun:/dev/net/tun

    ports:

      - 6881:6881

      - 6881:6881/udp

\#     - Add all other ports required by the different apps here

    volumes:

      - </path/to/your/gluetun\>:/gluetun

    environment:

      - VPN\_SERVICE\_PROVIDER=<your provider>

      - VPN\_TYPE=<wireguard or openvpn\>

      \# OpenVPN:

      \# - OPENVPN\_USER=

      \# - OPENVPN\_PASSWORD=

      \# Wireguard:

      - WIREGUARD\_PRIVATE\_KEY=<your-private-key>

      - WIREGUARD\_ADDRESSES=<your-wireguard\-adress\>

      - DNS=<your-wireguard\-dns\>

      - SERVER\_HOSTNAMES=<your-hostnames>

      - SERVER\_CITIES=<your-cities>

      - HTTPPROXY=off #change to on if you wish to enable

      - SHADOWSOCKS=off #change to on if you wish to enable

      \# Timezone for accurate log times

      - TZ=<your-timezone\>

      \# Server list updater

      \# See https://github.com/qdm12/gluetun-wiki/blob/main/setup/servers.md#update-the-vpn-servers-list

      - UPDATER\_PERIOD=24h

      - FIREWALL\_OUTBOUND\_SUBNETS=<synobridge-subnet>/16,<host-machine-subnet>/24 #change this in line with your subnet see note on guide

\#      - FIREWALL\_VPN\_INPUT\_PORTS=12345 #uncomment or remove this line based on the notes below

    network\_mode: synobridge

    labels:

      - com.centurylinklabs.watchtower.enable\=false

    security\_opt:

      - no-new-privileges:true

    restart: always

We have a lot to unpack here. So let�s just begin:

#### Ports

It is in the �ports:� section we put in all the network ports we are going to use. When we look at each of the official docker-compose.yml to all the different apps, they have their ports listed under their own service. However, since we are going to use a VPN, we need it to be in the GlueTUN network.

#### Volumes

Here we put the path to the folder we made earlier. If you only have one volume on your Synology and followed the same naming scheme as me, it should be �/volume1/docker/arr\-stack/gluetun�. Then we mount it as �/gluetun� by adding a �:�. So the full volume mapping should be �/volume1/docker/arr\-stack/gluetun:/gluetun�.

Note: Linux systems expect the use of a forward slash (/), and not backwards slash like in Windows (\\).

#### Environment

It�s in the environment we put in all the configuration settings.

##### VPN Service provider

�In the �VPN\_SERVICE\_PROVIDER� you fill in your VPN provider.

Here you can see a list of all the supported providers, as well as how to configure them:  
[https://github.com/qdm12/gluetun-wiki/tree/main/setup/providers](https://github.com/qdm12/gluetun-wiki/tree/main/setup/providers)

As I have only used Mullvad, AirVPN, and Privado, those are what I will show in detail how to setup.

You can also choose whether to use the WireGuard or OpenVPN protocol. In this example, we are using WireGuard as that is what I have found to work best. Except for Privado, which only offers OpenVPN for GlueTUN at the time of writing. But beware, the OpenVPN protocol is slow and resource demanding.

If you don�t use Mullvad, AirVPN or Privado, you will have to find out yourself how to configure GlueTUN for your provider. The official docs and ChatGPT will be your friend here. Skip to [Page 42](#_Proxy) to continue. But if you are using either Mullvad, AirVPN or Privado, you can follow my guide:

###### Mullvad

1.      Go to this link and put in your account number: [https://mullvad.net/no/account/wireguard-config](https://mullvad.net/no/account/wireguard-config)

2.      Click on �Generate Key� **Note:** The displayed key is NOT the private key.

3.      Choose a country, city and then the servers you wish to use. I have selected Sweden, Stockholm and all servers.

4.      Click �Download zip-archive�

0![Et bilde som inneholder tekst, skjermbilde, programvare, Nettside
Automatisk generert beskrivelse](media-filer/image021.png)

5.      Inside the zip file, you will find a bunch on .conf files. (Might be .json files) Open these in notepad.

6.      You only need one of them, as the relevant information is the same in every single one. You need to look at your \[Interface\] section and copy your �PrivateKey� as well as �Address� and �DNS�.

![Et bilde som inneholder tekst, skjermbilde, Font
Automatisk generert beskrivelse](media-filer/image022.png)

So for this example I would have to use:

�iExD5V5kkXnh+40dyo/PmCL1aus8eNBdHQMWergYFWo=� as my private key,

��10.72.171.113/32� as my address and

�10.64.0.1� as my DNS.

7.      Also take note of the filenames. They should be something like �se-sto-wg-001.conf�, where �se� is the country, �sto� the city and �wg� the protocol. So, for me it�s Sweden, Stockholm, WireGuard.

###### AirVPN

1.      Login to AirVPN and head over to �Client Area�. Click on �Manage� under �VPN Devices�. Or you can click this link:

[https://airvpn.org/devices/](https://airvpn.org/devices/)

2.      Click on �Add new device�. Call it something you will remember. For me, I went with GlueTUN. The name doesn�t really matter.

3.      Head back to �Client Area�, and this time select �Config Generator�. Or follow this link: [https://airvpn.org/generator/](https://airvpn.org/generator/)

4.      Select Linux as OS and WireGuard as Protocol. Select the server you want to use. For simplicity, I will just go for �Cepheus� in Norway. Scroll all the way down and click on �Generate.� A download of a text file should start. If you have selected multiple server, you might need to scroll all the way up where you will find a download for each one.

5.      The .conf text file should look kind of like this (Not my actual details, I changed them)

![Et bilde som inneholder tekst, skjermbilde, Font
Automatisk generert beskrivelse](media-filer/image023.png)

Now we can start to fill in the information in our docker-compose variables:

 - VPN\_SERVICE\_PROVIDER=airvpn

      - VPN\_TYPE=wireguard

      - WIREGUARD\_PRIVATE\_KEY=iEIR+vLDwV9KSqC+j1VxolEZ4WhlHvDMXIv20AwKXFw=

      - WIREGUARD\_PRESHARED\_KEY=//QhNVyHOGTXOB0by0sZ/OZj9PSTwFZ8yI6OiDg+6OY=

      - WIREGUARD\_ADDRESSES=10.184.194.25/32

      - DNS=10.128.0.1,1.1.1.1,fd7d:76ee:e68f:a993::1

      - SERVER\_HOSTNAMES=

      - SERVER\_REGIONS=Europe

      - SERVER\_COUNTRIES=Norway

      - SERVER\_CITIES=Oslo

If you want to, you can do like me and add more DNS servers. I also added CloudFares 1.1.1.1. Just remember to separate it with a �,�(comma). Same goes for the server regions, countries and cites. If you have multiple, list all of them with a �,�(comma) separating each one. Kind of like this:

      - SERVER\_COUNTRIES=Norway,Sweden,Denmark

Now we just need to find out our server hostname(s). It does not say in the config file, so to find the server hostname we will have to go to github and look at the source code:

[https://raw.githubusercontent.com/qdm12/gluetun/refs/heads/master/internal/storage/servers.json](https://raw.githubusercontent.com/qdm12/gluetun/refs/heads/master/internal/storage/servers.json).

Use ctrl+f (Search) and search for your server name. For me it was �Cepheus�. For �Cepheus� we have 6 results. You can find the hostname under: "hostname": "no3.ipv6.vpn.airdns.org". So for this server it is �no3.ipv6.vpn.airdns.org�. Select as many as you want, I would say atleast 2-3 so if one goes offline you won�t get disconnected, then put them in the docker-compose with comma separating each one.

![Et bilde som inneholder tekst, skjermbilde, Font
Automatisk generert beskrivelse](media-filer/image025.png)

###### PrivadoVPN

For PrivadoVPN we will have to use OpenVPN. Even though PrivadoVPN supports WireGuard now, GlueTUN does not support Privado with WireGuard. The country selection pool is also not that when it come sto GlueTUN support. But the good thing about OpenVPN is that it�s a whole lot easier to setup. You won�t need to download anything, nor find hostnames anywhere. This is how you do it:

1.      Copy-Paste this into your docker-compose:

      - VPN\_SERVICE\_PROVIDER=privado

      - VPN\_TYPE=openvpn

      - VPN\_DISABLE\_IPV6=true

      - OPENVPN\_USER=

      - OPENVPN\_PASSWORD=

      - SERVER\_COUNTRIES=

      \- SERVER\_CITIES=

2.      Fill in your PrivadoVPN username and password.

3.      Fill in your desired Country and City. I would recommend Netherlands, Germany or Hungary Amsterdam as I know this is supported aswell as it�s in the EU. The server being in the EU means that the government can�t access any logs or anything like that by EU law (GDPR), which means that it�s much more secure and private.

The only available servers for PrivadoVPN with GlueTUN are:

1.      Germany, Frankfurt.

2.      Hungary, Budapest,

3.      Netherlands, Amsterdam

4.      United States, Los Angeles

5.      United States, Washington

6.      United States, North Potomac

7.      United States, Ashburn

  

##### Proxy

If you are using a proxy, you can enable httpproxy and shadowsocks. I have not used it and will therefore not go over that now.

##### Timezone

In the timezone you just put in your own timezone. To find your TZ format, find your region in this list:  
[https://en.wikipedia.org/wiki/List\_of\_tz\_database\_time\_zones](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)

#### Firewall Outbound Subnets

In this line:

�FIREWALL\_OUTBOUND\_SUBNETS=<your-bridge-subnet>/,<your-host-subnet>�

We need to change the first IP to the one we just made for our synobridge. If you followed me, it will be 172.20.0.0/16. Then we will need to fill in our host machines subnet,

We have a few choices on how to identify it. If you are connected to the same network on your PC or phone, you can just figure out your IP address on your device of choice. So, for PC, open �cmd� and type �ipconfig�. Look for IPv4 section.

�If you have an iPhone, you can open settings >Wi-Fi > i (next to the Wi-Fi named) then scroll down to find the �IP address� field under �IPv4 address�

The IPv4 address will probably be something like this �192.168.X.X�. Take the first 3 digits, e.g. �192.168.0� or whatever you have, then replace the last digit with a 0. So if your IP address on your phone is �192.168.0.53� the subnet would be �192.168.0.0�. Then we just add the network mask at the end. If you don�t know what that means, it�s probably /24 at the end, so the full subnet is �192.168.0.0/24�.

So, my line would look like this:  
  

�FIREWALL\_OUTBOUND\_SUBNETS=172.20.0.0/16,192.168.0.0/24�

#### Network\_mode

We need to specify the network we made. If you gave it the same name as me, it should be �synobridge�.

####     labels: - com.centurylinklabs.watchtower.enable\=false

These lines just makes it so Watchtower doesn�t update it automatically. The reason we don�t want it to update is because it will break the whole arr\-stack each time. So the best practice would be to just leave it in. You can always manually update it when you want.

####     security\_opt: - no-new-privileges:true:

Makes it so the container can�t gain any more privileges than they are assigned, and makes it more secure. Probably best to include on every container.

#### Restart: always

This line tells the container to restart if it shuts down unexpectedly.

#### Full GlueTUN docker-compose.yml

With all of the info above, I now need you to make the appropriate edits for your docker-compose. This will be mine for this example:

  

gluetun:

    image: qmcgaw/gluetun

    container\_name: gluetun

    hostname: gluetun

    cap\_add:

      \- NET\_ADMIN

    devices:

      - /dev/net/tun:/dev/net/tun

    ports:

      - 6881:6881

      - 6881:6881/udp

      \- 8085:8085 \# qbittorrent

      - 8989:8989 \# Sonarr

      - 9696:9696 \# Prowlarr

      - 7878:7878 \# Radarr

      - 8686:8686 #Lidarr

      - 8191:8191 #FlareSolverr

      \- 5055:5055 #Overseer

      - 4545:4545 #Requestrr

    volumes:

      - \\volume1\\docker\\arr\-stack\\gluetun:/gluetun

    environment:

      - VPN\_SERVICE\_PROVIDER=mullvad

      - VPN\_TYPE=wireguard

      - VPN\_DISABLE\_IPV6=true

      \# OpenVPN:

      \# - OPENVPN\_USER=

      \# - OPENVPN\_PASSWORD=

      \# Wireguard:

      - WIREGUARD\_PRIVATE\_KEY= iExD5V5kkXnh+40dyo/PmCL1aus8eNBdHQMWergYFWo=

      \- WIREGUARD\_ADDRESSES=10.72.171.113/32

      - DNS=10.64.0.

      - SERVER\_HOSTNAMES=se-sto-wg-001,se\-sto-wg-002,se-sto-wg-003,se-sto-wg-004

      \- SERVER\_CITIES=stockholm

      - HTTPPROXY=off #change to on if you wish to enable

      - SHADOWSOCKS=off #change to on if you wish to enable

      \# Timezone for accurate log times

      - TZ=Europe/Oslo

      - UPDATER\_PERIOD=24h

      - FIREWALL\_OUTBOUND\_SUBNETS=172.20.0.0/192.168.0.0/24

    network\_mode: synobridge

    labels:

      - com.centurylinklabs.watchtower.enable\=false

    security\_opt:

### Download client

The best torrent download client in my opinion is qBitTorrent and is therefore what I will use today. But you can use rTorrent or any other preferred torrent client. Here is the docker-compose for qBitTorrent:

qbittorrent:

    image: lscr.io/linuxserver/qbittorrent

    container\_name: qbittorrent

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=<your-timezone\>

      - WEBUI\_PORT=8085

      - UMASK=022

    volumes:

      - /path/to/your/config:/config

      - /path/to/your/media/torrents:/Media/Torrents

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: always

#### network\_mode

If you also are using a VPN, and therefore by extension gluetun, you will need to set network\_mode to �service:gluetun�. If you don�t use VPN, you can just do �network\_mode: bridge� or any other network you have set up.

#### Environment

##### PUID and PGID

For PUID and PGID you need to find the ID for your user. To do this, SSH into your Synology, log in to your own user, then type �id�. The output should include UID (user ID) and GID (Group ID).

##### UMASK

I simply don�t have enough information on this to tell you what it is or how it works. If you are interested, you can read here: [https://en.wikipedia.org/wiki/Umask](https://en.wikipedia.org/wiki/Umask)

##### Volumes

If you followed me in the creation of the directories, it should be:  
  
/volume1/docker/arr\-stack/qbittorrent/config:/config

/volume1/Media//orrents:/Media/Torrents

**NOTE:** It is very important that we have torrents in the same shared folder as our media library. This is because of how hardlinks work. If we do not have it in the same folder, we will then copy the files. So, for every 10GB file, you would have to use 20GB of storage. This adds up really quickly to many TBs of wasted storage.

#### Full docker-compose.yml for qbittorrent

The full docker-compose could look something like this:

qbittorrent:

    image: lscr.io/linuxserver/qbittorrent

    container\_name: qbittorrent

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

      - WEBUI\_PORT=8085

      - UMASK=022

    volumes:

      - /volume1/docker/arr\-stack/qbittorrent/config:/config

      - /volume1/Media/Torrents:/media/Torrents

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: always

  

### Sonarr

This is the docker-compose.yml

sonarr:

    image: lscr.io/linuxserver/sonarr:latest

    container\_name: sonarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    volumes:

      - /path/to/your/config:/config

      - /path/to/your/media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

We have already covered most of the components in the docker-compose file, so I won�t repeat myself. The only thing I want to mention is the fact that if you separate your TV shows and Anime shows in your Media folder, like me, you need to mount both of them here.

#### Something important:

The path to your media **NEED** to be in the same shared folder as the torrents, for the reason we talked about earlier.

  

#### Full docker-compose.yml file

sonarr:

    image: lscr.io/linuxserver/sonarr:latest

    container\_name: sonarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/sonarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  

### Radarr

Here we have Radarr�s docker-compose:

radarr:

    image: lscr.io/linuxserver/radarr:latest

    container\_name: radarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/radarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

So, as you can see, it�s identical to Sonarr�s, except for the image and name.

  

### Lidarr

Docker-compose:

lidarr:

    image: lscr.io/linuxserver/lidarr:latest

    container\_name: lidarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/lidarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

Again, we have a pretty familiar looking docker-compose file. Edit the appropriate settings just like you did for Radarr.

  

### Prowlarr

Prowlarr is what we use connect our indexers to our apps. Here is the docker-compose:

  prowlarr:

    image: lscr.io/linuxserver/prowlarr:latest

    container\_name: prowlarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=<your-UID>

      - PGID=<your-GID>

      - TZ=Europe/Oslo

    volumes:

      - /path/to/your/config:/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

Obviously change the PUID and PGID. Other than that, we only have to change the config path. It should be �/volume1/docker/arr\-stack/prowlarr/config:/config�.

  

### Flaresolverr

**NOTE**: This does not work anymore.

[https://trash-guides.info/Prowlarr/prowlarr-setup-flaresolverr/](https://trash-guides.info/Prowlarr/prowlarr-setup-flaresolverr/)

Docker-compose:

flaresolverr:

    image: ghcr.io/flaresolverr/flaresolverr:latest

    container\_name: flaresolverr

    network\_mode: "service:gluetun"

    environment:

      - TZ=Europe/Oslo

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: unless-stopped

You don�t need to change anything here. Just paste it in. The only exception is if you don�t use VPN, then change �network\_mode� and delete �depends\_on�.

  

### Overseerr

Docker-compose:

 overseerr:

    image: sctx/overseerr:latest

    container\_name: overseerr

    network\_mode: "service:gluetun"

    environment:

      - LOG\_LEVEL=debug

      - TZ=Europe/Oslo

    volumes:

      - /path/to/your/config:/app/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

The only thing you need to change here is the path to your config. It should be �/volume1/docker/arr\-stack/overseer/config:/app/config�

  

### Requestrr

Docker-compose:

 requestrr:

    image: darkalfx/requestrr

    container\_name: requestrr

    network\_mode: "service:gluetun"

    volumes:

    - /path/to/your/config:/root/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  
Again, only change the config path. Should be

��\\volume1\\docker\\arr\-stack\\requestrr\\config�

  

### Tautulli

Docker-compose:

  tautulli:

    image: ghcr.io/tautulli/tautulli

    container\_name: tautulli

    network\_mode: service:gluetun #Replace this bridge if you don�t use GlueTUN

    restart: unless-stopped

    volumes:

      - /path/to/your/config:/config

    environment:

      - PUID=<your UID>

      - PGID=<your GID>

      - TZ=Europe/Oslo

    depends\_on: #use this if you use GlueTUN for VPN

      gluetun:

        condition: service\_healthy

For me it would look like this:

  tautulli:

    image: ghcr.io/tautulli/tautulli

    container\_name: tautulli

    network\_mode: service:gluetun

    restart: unless-stopped

    volumes:

      - /volume1/docker/arr\-stack/tautulli/config:/config

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    depends\_on:

      gluetun:

        condition: service\_healthy

  

### Putting it all together

Now we can put all our relevant docker-compose files together inside one big file. Remember, if you want to add more \*arr apps or other download-clients, you can just add them in this docker-compose just like we did for all the other apps. Just remember to open up the ports in GlueTUN as well. For me the docker-compose.yml is like this:

version: "3"

services:

  gluetun:

    image: qmcgaw/gluetun

    container\_name: gluetun

    hostname: gluetun

    cap\_add:

      - NET\_ADMIN

    devices:

      \- /dev/net/tun:/dev/net/tun

    ports:

      - 6881:6881

      - 6881:6881/udp

      \- 8085:8085 \# qbittorrent

      - 8989:8989 \# Sonarr

      - 9696:9696 \# Prowlarr

      - 7878:7878 \# Radarr

      - 8686:8686 #Lidarr

      - 8191:8191 #FlareSolverr

      \- 5055:5055 #Overseerr

      - 4545:4545 #Requestrr

    volumes:

      - \\volume1\\docker\\arr\-stack\\gluetun:/gluetun

    environment:

      - VPN\_SERVICE\_PROVIDER=mullvad

      - VPN\_TYPE=wireguard

      - VPN\_DISABLE\_IPV6=true

      \# OpenVPN:

      \# - OPENVPN\_USER=

      \# - OPENVPN\_PASSWORD=

      \# Wireguard:

      - WIREGUARD\_PRIVATE\_KEY= iExD5V5kkXnh+40dyo/PmCL1aus8eNBdHQMWergYFWo=

      \- WIREGUARD\_ADDRESSES=10.72.171.113/32

      - DNS=10.64.0.

      - SERVER\_HOSTNAMES=se-sto-wg-001,se\-sto-wg-002,se-sto-wg-003,se-sto-wg-004

      \- SERVER\_CITIES=stockholm

      - HTTPPROXY=off #change to on if you wish to enable

      - SHADOWSOCKS=off #change to on if you wish to enable

      \# Timezone for accurate log times

      - TZ=Europe/Oslo

      \# Server list updater

      \# See https://github.com/qdm12/gluetun-wiki/blob/main/setup/servers.md#update-the-vpn-servers-list

      - UPDATER\_PERIOD=24h

      - FIREWALL\_OUTBOUND\_SUBNETS=172.20.0.0/192.168.0.0/24 #change this in line with your subnet see note on guide

\#      - FIREWALL\_VPN\_INPUT\_PORTS=12345 #uncomment or remove this line based on the notes below

    network\_mode: synobridge

    labels:

      - com.centurylinklabs.watchtower.enable\=false

    security\_opt:

  qbittorrent:

    image: lscr.io/linuxserver/qbittorrent

    container\_name: qbittorrent

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

      - WEBUI\_PORT=8085

      - UMASK=022

    volumes:

      - /volume1/docker/arr\-stack/qbittorrent/config:/config

      - /volume1/Media/Torrents:/Media/Torrents

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: always

  sonarr:

    image: lscr.io/linuxserver/sonarr:latest

    container\_name: sonarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/sonarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  prowlarr:

    image: lscr.io/linuxserver/prowlarr:latest

    container\_name: prowlarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/prowlarr/config:/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  radarr:

    image: lscr.io/linuxserver/radarr:latest

    container\_name: radarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/radarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  lidarr:

    image: lscr.io/linuxserver/lidarr:latest

    container\_name: lidarr

    network\_mode: "service:gluetun"

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/lidarr/config:/config

      - /volume1/Media:/Media

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  flaresolverr:

    image: ghcr.io/flaresolverr/flaresolverr:latest

    container\_name: flaresolverr

    network\_mode: "service:gluetun"

    environment:

      - TZ=Europe/Oslo

    depends\_on:

      gluetun:

        condition: service\_healthy

    security\_opt:

      - no-new-privileges:true

    restart: unless-stopped

  overseerr:

    image: sctx/overseerr:latest

    container\_name: overseerr

    network\_mode: "service:gluetun"

    environment:

      - LOG\_LEVEL=debug

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/overseer/config:/app/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  requestrr:

    image: darkalfx/requestrr

    container\_name: requestrr

    network\_mode: "service:gluetun"

    volumes:

    - /volume1/docker/arr\-stack/requestrr/config:/root/config

    depends\_on:

      gluetun:

        condition: service\_healthy

    restart: unless-stopped

  tautulli:

    image: ghcr.io/tautulli/tautulli

    container\_name: tautulli

    network\_mode: service:gluetun

    restart: unless-stopped

    volumes:

      - /volume1/docker/arr\-stack/tautulli/config:/config

    environment:

      - PUID=1026

      - PGID=100

      - TZ=Europe/Oslo

    depends\_on:

      gluetun:

        condition: service\_healthy

  

### Common Errors

The most common error to get now is �gluetun is unhealthy� If you get this, it is likely an error in the config file. Usually, it relates to the provider specific elements. If you check the logs for the GlueTUN container it will tell you why it couldn�t connect. My best guess would be incorrect private key, incorrect hostnames or something similar. If you can�t figure it out, please drop a comment or DM me with your logs, and I�ll take a look.

Also please, please, please! Double check the volume mounts. If they are not correctly set up, you will lose **HALF** your storage space to waste. It should be as follows:

Media

├── Torrents

│�� ├── Incomplete

│�� └── Complete

│������ ├── Movies

│������ ├── Music

|������� ├── Anime TV Shows

│������ └── TV Shows

├── Usenet

│�� ├── Incomplete

│�� └── Complete

│������ ├── Movies

│������ ├── Music

|������� ├── Anime TV Shows

│������ └── TV Shows

└── Media

��� ├── Movies

��� ├── Music

��� ├── Anime TV Shows

��� └── TV Shows

Configuration of the apps
=========================

qBitTorrent
-----------

### Login

The first thing we should do is configure qBitTorrent. Open a web browser (on your computer) then type in your NAS IP address followed by port 8085. For this example, it would look like this: 192.168.0.2:8085

You will then get to the login page for the qBitTorrent WebUI. The username is always admin. The password could be adminadmin, as this is the default. But most likely you will find a temporary password in the logs for the qBitTorrent container inside container manager.

![Et bilde som inneholder tekst, skjermbilde, Font, line
Automatisk generert beskrivelse](media-filer/image027.jpg)

  

### Change username and password

The first thing to do now that you are logged in is to change your username and password.� Click the cog icon at the top of the page, then go to the Web UI tab. Put in your new details then click save at the bottom of the page.

**NOTE:** Please change both your username and password for maximum security.

![Et bilde som inneholder tekst, skjermbilde, programvare, nummer
Automatisk generert beskrivelse](media-filer/image029.jpg)

  

### Change downloads path

Go back to settings, then go to the �Downloads� tab.

Change the default save path to �/Media/Torrents/Complete� and tick the box for �Keep incomplete torrents in:�. Select �/Media/Torrents/Incomplete�

![Et bilde som inneholder tekst, skjermbilde, programvare, nummer
Automatisk generert beskrivelse](media-filer/image031.png)

  

Radarr
------

### Adding Authentication method

Open a web browser on your PC, then type in the IP of your NAS followed by port 7878. So e.g. 192.168.0.2:7878. The first time you open this, you will be prompted to add an authentication method. I recommend using forms and having it enabled. Set username to something else than admin or administrator as this is easy to guess.

![Radarr Synology NAS Set up 3 new 2024](media-filer/image033.jpg)

  

### Adding Root Folder

Now go to settings on the left-hand side menu.

![Radarr Synology NAS Set up 4 new 2024](media-filer/image035.jpg)

Now go to media management, scroll down and click on �Add Root Folder�. Type /Media/Media/Movies and select it. Click OK.

![Radarr Synology NAS Set up 5 new 2024](media-filer/image037.jpg)

  

### Changing Movie Naming Scheme

1.      Go to settings, then choose media management. Turn on advanced settings (right under the search bar).

2.      Tick the box next to �Rename Movies� and �Replace illegal characters.�

3.      Change the �Standard Movie Format� to the one that fits you the best on TRaSH�s website. For Plex, I recommend to stick with Plex (TVDB). You can read more about recommended naming schemes here: [https://trash-guides.info/Radarr/Radarr-recommended-naming-scheme/](https://trash-guides.info/Radarr/Radarr-recommended-naming-scheme/)

4.      For Movie Folder Format I would go for �{Movie CleanTitle} ({Release Year}) {tmdb\-{TmdbId}}�, but again you can read more on TRaSH Guides.

![Et bilde som inneholder tekst, skjermbilde, programvare, Nettside
Automatisk generert beskrivelse](media-filer/image039.png)

5.      Make sure �Use Hardlinks instead of Copy� under �Importing� is enabled.

6.      Scroll down until you get to �File Management� and select �Do Not Prefer for� �Propers and Repacks�. This is important for our quality profiles later.

![Et bilde som inneholder tekst, programvare, Nettside, Nettsted
Automatisk generert beskrivelse](media-filer/image041.png)

Now be sure to click save, next to the �Show advanced� switch under the search bar.

  

### Quality Settings (File Size)

1.      Go to settings, then select �Quality� from the menu. Make sure to enable �Show Advanced� by clicking the cog under the search bar.

2.      Go to TRaSH Guids and change the appropriate settings as described for the best quality settings. You can edit these at will to save storage space.

[https://trash-guides.info/Radarr/Radarr-Quality-Settings-File-Size/](https://trash-guides.info/Radarr/Radarr-Quality-Settings-File-Size/)

![Et bilde som inneholder tekst, skjermbilde, programvare, Dataikon
Automatisk generert beskrivelse](media-filer/image043.png)

  

### Quality profiles

1.      Go to settings, Profiles.

![!cf-settings-profiles](media-filer/image044.png)

2.      Delete all the default ones.

3.      Create a new one

4.      Go to TRaSH Guide�s and follow their instructions on how to setup quality profiles, aswell as to set custom formats. Add all the profiles you need for your setup�s needs and wants.

[https://trash-guides.info/Radarr/radarr-setup-quality-profiles/](https://trash-guides.info/Radarr/radarr-setup-quality-profiles/)

  

Sonarr
------

### Adding Root Folder(s)

1.      Open a web browser on your PC and type in the IP of your NAS followed by port 8989. So e.g. 192.168.0.2:8989.

2.      Here you will be prompted to set up an authentication method. I recommend selecting �Forms� and having it enabled. Choose a username that is not admin or administrator, then select a password.

![Sonarr Synology NAS Set up 6 new 2024](media-filer/image046.jpg)

3.      Go to settings

![Sonarr Synology NAS Set up 7 new 2024](media-filer/image048.jpg)

4.      Select �Media Management�, scroll down and click on �Add Root Folder�. Type in �/Media/Media/TV Shows/� and select it before you click OK. If you have a separate folder for anime, add another root folder and search for �/Media/Media/Anime TV Shows� and select it. Click OK.

![Sonarr Synology NAS Set up 8 new 2024](media-filer/image050.jpg)

  

### Changing Naming Scheme(s)

1.      Go to settings > Media Management and click on Show Advanced.

![Enable Advanced](media-filer/image051.png)

2.      Enable �Rename Episodes�. I recommend to also enable �Replace illegal characters�

![Enable Rename Episodes](media-filer/image053.png)

3.      Go to TRaSH Guide�s and select the settings they recommend.

[https://trash-guides.info/Sonarr/Sonarr-recommended-naming-scheme/#standard](https://trash-guides.info/Sonarr/Sonarr-recommended-naming-scheme/#standard)

4.      Scroll down to �File Management� and select �Do not Prefer� for �Propers and Repacks�. This is important for our quality profiles later.

5.      Under �Importing� make sure �Use Hardlinks instead of Copy� is enabled.

  

### Quality Settings (File Size)

1.      Go to settings and select �Quality�

2.      Enabled �Show Advanced� by clicking the cog at the top.

3.      Go to TRaSH Guides and edit the appropriate settings for the best quality.

[https://trash-guides.info/Sonarr/Sonarr-Quality-Settings-File-Size/](https://trash-guides.info/Sonarr/Sonarr-Quality-Settings-File-Size/)

![Et bilde som inneholder tekst, skjermbilde, programvare, Dataikon
Automatisk generert beskrivelse](media-filer/image055.png)

  

### Quality Profiles

1.      Go to settings and select �Profiles�

![!cf-settings-profiles](media-filer/image056.png)

2.      Delete all the default ones.

3.      Go to TRaSH Guides and set up profiles as described there. Import the relevant custom formats that fit your needs and wants.

[https://trash-guides.info/Sonarr/sonarr-setup-quality-profiles/](https://trash-guides.info/Sonarr/sonarr-setup-quality-profiles/)

  

### Quality Profiles (Anime)

1.      Go to settings and select �Profiles�

![!cf-settings-profiles](media-filer/image056.png)

2.      Delete all the default ones.

3.      Go to TRaSH Guides and set up profiles as described there. Import the relevant custom formats that fits your needs and wants.

[https://trash-guides.info/Sonarr/sonarr-setup-quality-profiles-anime/](https://trash-guides.info/Sonarr/sonarr-setup-quality-profiles-anime/)

  

Lidarr
------

### Adding Root Folder(s)

1.      Open a web browser on your PC and type in the IP of your NAS followed by port 8686. So e.g. 192.168.0.2:8686.

2.      Here you will be prompted to set up an authentication method. I recommend selecting �Forms� and having it enabled. Choose a username that is not admin or administrator, then select a password.

![Lidarr Synology NAS Set up 6 new 2024](media-filer/image058.jpg)

3.      Go to settings, then select �Media Management�.

4.      Click on the big �+� sign under �Add Root Folder

![Lidarr Synology NAS Set up 8 new 2024](media-filer/image060.jpg)

5.      Search for �/Media/Media/Music� select it then click on OK

![Lidarr Synology NAS Set up 9 new 2024](media-filer/image062.jpg)

6.      Make sure �Rename Tracks� and �Replace illegal characters� are enabled.

![Et bilde som inneholder tekst, skjermbilde, programvare, Nettside
Automatisk generert beskrivelse](media-filer/image064.png)

�Standard Track Format� should be:

{Album Title} ({Release Year})/{Artist Name} - {Album Title} - {track:00} - {Track Title}

And �Multi Track Format� should be:

{Artist Name}/{Album Title} ({Release Year})/{Medium Format} {medium:00}/{Artist Name} - {Album Title} - {track:00} - {Track Title}

  

### Quality Settings

TRaSH Guides have no guides on lidarr. I have tried to search the internet but have not found any guides on quality settings or profiles for lidarr. I have only set up one profile myself on Lidarr, which is a pretty basic one without any scoring systemor custom formats. I have also not changed the size for the different Quality Settings.

![](media-filer/image066.png)

  

Connecting download client to Radarr, Sonarr and Lidarr
-------------------------------------------------------

Now that we have configured all our main arr\-apps, we need to actually give them something to send the downloads to. For this guide we are using qBitTorrent. The setup will be identical for all of the apps, so just repeat the steps for all of them.

1.      Go to settings, then select �Download Clients�

2.      Make sure �Automatically import completed downloads from download client� is enabled.

3.      Click on the big �+� icon.

![Et bilde som inneholder tekst, skjermbilde, programvare, Dataikon
Automatisk generert beskrivelse](media-filer/image068.png)

4.      Select qBitTorrent

5.      Fill out the details

i.                    ��Name: qBitTorrent

ii.                  �Enable

iii.                �Host: 170.20.0.2

�**NOTE:** This must be the IP of the **GlueTUN** container, and **NOT** the NAS itself. So instead of 192.168.0.2, we put 172.20.0.2. To confirm this is the correct IP, we can go back to Synology container manager > container and click on gluetun. Scroll down until you find �Network Settings� and look for where is says �IP Address�

![Et bilde som inneholder tekst, nummer, line, skjermbilde
Automatisk generert beskrivelse](media-filer/image070.png)

iv.                �Port: 8085

v.                  �Username: <username on qBitTorrent\>

vi.                �Password: <password on qBitTorrent\>

vii.               �Category: <the appropriate category. music/movies/tv/anime>

������������������������������ **NOTE:** For Sonarr, you will need to setup 2 download clients if you want to

separate anime to a separate folder than tv. Both can be the same

client, with identical setup. Only thing that must change is the

�Category� has to be �anime� for anime and �tv� or �series� for

normal TV Series.

6.      Click �Test�. If it becomes green for a second, then press �Add� If it becomes red, review and double check your settings.

![](media-filer/image072.png)

  

Prowlarr
--------

### Adding the apps to Prowlarr

Now that we have set up all our downloaders, we need something to search for the files we are going to download. For that, we will use Prowlarr for best control.

1.      Go to <NAS-IP>:9696 e.g. 192.168.0.2:9696

2.      Fill out the form just like earlier.

![Prowlarr Synology NAS Set up 6 new 2024](media-filer/image074.jpg)

3.      Go to settings on the left-hand side menu.

![Prowlarr Synology NAS Set up 7 new 2024](media-filer/image076.jpg)

4.      Click on apps, then the big �+� under applications

![Prowlarr Synology NAS Set up 8 new 2024](media-filer/image078.jpg)

5.      Click on the app you want. We can start with Radarr.

![Prowlarr Synology NAS Set up 9 new 2024](media-filer/image080.jpg)

  

6.      Fill out the form:

\-          Name can be default.

\-          Sync Level: Full Sync

\-          Tags: Leave blank

\-          Prowlarr server: [http://172.20.0.2:9696](http://172.20.0.2:9696)

\-          Radarr server: [http://172.20.0.2:7878](http://172.20.0.2:7878)

**NOTE:** If you chose another IP for your �synobridge� network, then put that in instead.

\-          API Key: Get this from the relevant app. In this case, Radarr. Scroll down to find out how.

7.      Repeat this step for all the apps you want; LazyLibrarian, Lidarr, Mylar, Radarr, Readarr, Sonarr and Whisparr.

![Prowlarr Synology NAS Set up 10 new 2024](media-filer/image082.jpg)

  

### How do I get the API key?

1.      Open your relevant application in the browser.

2.      Go to settings, then click on �General�

3.      The API Key should be right there. Just click the copy button on the right, and paste that into Prowlarr.

![Prowlarr Synology NAS Set up 11 new 2024](media-filer/image084.jpg)

  

### Connecting Flaresolverr

Some indexers, like 1337x which is one of the best free ones, require you to solve a Cloudflare verification before you get access. To make prowlarr do this, you must use flaresolverr. To do this:

1.      Go to settings, then click on indexers

2.      Click the big + icon.

![Et bilde som inneholder skjermbilde, programvare, Multimedieprogramvare, datamaskin
Automatisk generert beskrivelse](media-filer/image086.png)

3.      Edit the �Host� field to be �http://172.20.0.2:8191�

![Et bilde som inneholder tekst, skjermbilde, nummer, Font
Automatisk generert beskrivelse](media-filer/image088.png)

4.      Click on �Test� and if it becomes green for a second it works, and you can click �Save�. If it becomes red, then double check your Host IP. It should be the same as your �synobridge� network in docker.

![Et bilde som inneholder tekst, Font, logo
Automatisk generert beskrivelse](media-filer/image089.png)

  

### Adding indexers

Indexers are the websites prowlarr search for files. Sadly, a lot of the good ones are private. This means that to use them you will most likely need to pay to get access or get invited. Therefore, I will focus on the free ones.

1.      Click on Indexers, then �Add Indexer�

![](media-filer/image091.png)

2.      Here can filter by protocol, Language, Privacy and Category. All indexers that use the �nzb� protocol are for UseNet and most of these are private. But this is for torrents, and we will therefore ignore them for now. You could just set the privacy to public to get a list of all the free ones. The ones I would recommend getting at least are 1337x and TheRARBG for general TV and movies, and Nyaa for anime.

3.      We can now search for our desired indexers, then click on the result

4.      Fill out the settings. Base URL should be 1337x.to and I would also recommend to tur non advanced settings, then choose �minimum seeders: 1�.

![Et bilde som inneholder tekst, skjermbilde, nummer, programvare
Automatisk generert beskrivelse](media-filer/image093.png)

�If we scroll down, we can see that it says it requires flaresolverr. Now we can click �Test� to see if it works, and if it does, we can click �Save�. Do this for all your wanted indexers.

![Et bilde som inneholder tekst, skjermbilde, Font, nummer
Automatisk generert beskrivelse](media-filer/image095.png)

5.      After you have added all your desired indexers, click on �Sync App Indexers� to push them to all your apps.

![Et bilde som inneholder tekst, skjermbilde, design
Automatisk generert beskrivelse](media-filer/image096.png)

6.      Let�s wait 2-5 minutes for it to finish up, then we can head into our apps, like Radarr or Sonarr, and click on settings > indexers to see our selected indexers with a (prowlarr) at the end to indicate where it comes from.

![Et bilde som inneholder tekst, skjermbilde, programvare, Font
Automatisk generert beskrivelse](media-filer/image098.png)

![Et bilde som inneholder tekst, skjermbilde, Font, logo
Automatisk generert beskrivelse](media-filer/image099.png)

  

Overseerr
---------

Now it�s time to take the automation to the next level. With overseer, we get a huge catalogue of movies and shows at our fingertips and can download them with just one click.

### Configuring Overseerr

1.      Go to <synolog-ip\>:5055.

2.      Click �Sign In�, and follow the sign in instructions

![Overseerr Synology NAS Set up 6 new](media-filer/image101.jpg)

3.      On the setup screen, **DON�T** use your synobridge but your **NAS** IP (same one yo use to access this website). So, for me it�s 192.168.0.2. If you haven�t changed the plex port, it can stay as default. Click �Save Changes�. You should now see a green checkmark at the top.

![Overseerr Synology NAS Set up 7 new](media-filer/image103.jpg)

4.      Scroll down a bit and click �Sync Libraries�. Afterwards you can click continue. If it�s not done syncing, it will continue in the background.

![Overseerr Synology NAS Set up 8 new](media-filer/image105.jpg)

5.      Add your Radarr and Sonarr by clicking the buttons as shown in the image below. Scroll down to continue.

![Overseerr Synology NAS Set up 9 new](media-filer/image107.jpg)

  

### Adding Radarr and Sonarr

On the first-time setup, you will get a prompt to add Radarr and Sonarr. If you manage to miss it, freight not as you can do it in settings later. Just head to settings > services then click on add.

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image109.png)

  

#### Radarr

1.      When you click on �Add Radarr Server� you should see something like this:

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image111.png)

2.      Fill out server name, hostname, port and API Key as follows:

\-          Server Name radar (or anything you like)

\-          Hostname: 170.20.0.2 (your synobridge IP)

\-          Port: Default. 7878 for Radar

\-          API Key: Your relevant API Key. Don�t know how to get it? Check the table of contents.

3.      Now click on �Test�. If it�s successful, you will now get to select the rest of the settings.

4.      Now configure the rest of the settings:

\-          Quality Profile: Your desired default quality profile. This can be changed every time you request in Overseer, but not in Requestrr

\-          Root folder: �/Media/Media/Movies�

\-          Minimum availability: Whatever you prefer. I want it to be released.

\-          Tick the options for �Enable scan� and �Enable Automatic Search�

![](media-filer/image113.png)

5.      Now we can save our changes.

  

#### Sonarr

1.      After you click �Add Sonarr�, you should see something like this:

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image115.png)

2.      Fill out the settings like this:

\-          Servername: sonarr (or anything you like)

\-          Hostname: 170.20.0.2 (Your synobridge IP)

\-          Port: Default. 8989 for Sonarr

\-          API Key: Your API Key. Don�t know where to get it? Check the table of contents.

3.      Now we can click �Test� to test out connection. If it�s successful, we can now move on to edit some more settings.

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image117.png)

4.      Now make these changes to the settings:

\-          Quality Profile: Your desired default quality profile. This can be changed every time you request in Overseer, but not in Requestrr

\-          Root Folder: �/Media/Media/TV Shows�

\-          Language Profile: Depricated

\-          Tags: series

\-          Anime Quality profile: Your desired default quality profile for anime shows. This can be changed every time you request in Overseer, but not in Requestrr

\-          Anime Root Folder: �/Media/Media/Anime TV Shows�

\-          Language Profile: Depricated

\-          Anime Tags: anime

\-          Be sure to tick the boxes for �Enable Scan� and �Enable Automatic Search�

5.      Click �Save�

![](media-filer/image119.png)

### Requestrr

Now we can configure Requestrr. It allows us, and our users, to request movies and TV shows through chat in discord. This is a good alternative if you don�t know how or don�t want to port forward your Overseer. Or if you plan to share your Plex with strangers and don�t want them to know your public IP-address

#### Configuring Requestrr

1.      Open Requestrr in a web browser by typing <NAS-IP>:4045

2.      The first time you log in, you might get a pop-up to create an authentication method just like all the other apps. Fill out the form like earlier then.

3.      When we open up Requestrr, we should see our Chat clients. If not, navigate to it on the left-hand side menu.

![Et bilde som inneholder tekst, skjermbilde, programvare, Dataikon
Automatisk generert beskrivelse](media-filer/image121.png)

4.      As you can see, we need an Application Id and Bot Token for Discord. Here is how you can get it:

#### How to get Discord Application Id and Bot Token

1.      Go to Discord Developer Portal by� clicking this link: [https://discordapp.com/developers/applications](https://discordapp.com/developers/applications)

2.      Click on New Application

![newapplication](media-filer/image123.png)

3.      Give it a name and a profile picture if you so wish. The important thing is to copy the Application Id.

![clientid](media-filer/image125.png)

4.      Paste it into Requestrr

![copyclientid](media-filer/image127.png)

5.      Go back into Discord Developer Portal and create a bot for your newly created application.

![createbot](media-filer/image129.png)

6.      Make sure these 2 settings are enabled:

![presenceintents](media-filer/image131.png)

7.      Now copy the Bot Token

![copybottoken](media-filer/image133.png)

8.      Paste the Bot Token into Requestrr

![pastebottoken](media-filer/image135.png)

9.      Click on �Test Settings� to check if the connection is good

![testsettings](media-filer/image137.png)

10. Go to your discord server, right click on the channel you want your bot to be in and copy the channel ID. Paste it into �Channel(s) to send notifications to�

![](media-filer/image139.png)

11. Finally, we can save our changes

![savechanges](media-filer/image140.png)

  

#### How to invite the bot to our Discord server

1.  Be sure you have created a Discord server, or are admin in an existing one

1.  Click �Copy Invite Link�

![copyinvitelink](media-filer/image142.png)

1.  Choose the Server you whish to add the Bot to

![invitebot](media-filer/image144.png)

  

#### Connecting Requestrr to Overseerr (Or Radarr, Sonarr, Ombi)

Now we have to set up Requestrr to actually, well, request. The best way would be to use Overseer or Ombi, but it also works directly with Radarr and Sonarr.

1.      Go to Overseer on your web-browser. <NAS-IP>:5055

2.      Go to settings (On the left-hand side menu) and make sure �Enable CSRF Protection� is disabled (unticked)

3.      While you�re here, also copy your Overseer API key.

![Et bilde som inneholder skjermbilde, tekst, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image146.png)

4.      Go to Requestrr on your web-browser. <NAS-IP>:4045

5.      Go to Movies (On the left-hand side menu)

![Et bilde som inneholder tekst, skjermbilde, programvare, Dataikon
Automatisk generert beskrivelse](media-filer/image148.png)

6.      Choose Overseer as Download Client. Paste in your API Key. Host should be 170.20.0.2 (your synobridge) and port 5055.Default Overseer user is which user the requests should come from. To find out your user ID to as follows:

i Go back to overseer

ii Select �Users� from the menu

iii Then you should see a list of all your users. I made a custom Requestrr user.

![](media-filer/image150.png)

Click on the desired user. Now you should see your user id

![](media-filer/image151.png)

7.      Click �Test Settings�, then scroll down and click on �Save Changes�

8.      Now go to �TV Shows� from the menu and do the exact same as you did for movies. Most of it should already be automatically filled out by your movies section when you select �Overseerr� as client.

9.      Now it works! You can go to your server and type /help in the channel you copied the ID for earlier, and it will list all available commands.

  

Modifications to set it up for UseNet
=====================================

FAQ
---

### What is Usenet?

Use(er) Net(work) is a worldwide distributed discussion system available on computers. It was developed from the general-purpose Unix-to-Unix Copy (UUCP) dial-up network architecture.

A major difference between a BBS or web message board and Usenet is the absence of a central server and dedicated administrator or hosting provider. Usenet is distributed among a large, constantly changing set of [news servers](https://en.wikipedia.org/wiki/News_server "News server") that [store and forward](https://en.wikipedia.org/wiki/Store_and_forward "Store and forward") messages to one another via "news feeds".

\-Wikipedia. [https://en.wikipedia.org/wiki/Usenet](https://en.wikipedia.org/wiki/Usenet) �

### What is UseNet used for

In simple terms, when UseNet was created, it was meant to share news and messages, kind of like what reddit is today. But today it is (almost) only used to share media content.

### Why are the files split into parts?

Usenet is a text forum. Message size is limited to 1 million bytes. A binary file must be split into pieces smaller than 1 million bytes. Each of these segments is a Usenet message.

### Do I need to manually combine all the parts of the files afterwards?

You download an NZB file from your indexer. The NZB file contains a list of files, and a list of Message-IDs for each file. Your download client (newsreader) uses the NZB to download all the messages and reassemble the original file(s).

  

 

### UseNet vs Torrenting for Media Downloads

Some will argue UseNet is better in every way, and in a lot of cases it is. But it isn�t as black and white as this. UseNet will offer much greater speeds, often maxing out your ISP speed of 500Mbps/1Gbps/2.5Gbps. You will also not be dependent on seeders, or to be seeding yourself.

One thing to point out is the aspect of retention. Files are only stored so long on the file server. This is often about 10-15 years depending on provider but reposts happen all the time so it�s not such a big issue. Another thing is that not all backbones (fileservers) have all the files. Therefore, even though an indexer could grab it you won�t have all the files to complete a download. Another downside is that it costs money. All providers cost money, and most indexers do aswell. Some indexers have free trials and/or free plans though but keep a lookout for sales and deals.

To find some good deals, check out the wiki on reddit:

Providers: [https://www.reddit.com/r/usenet/wiki/providerdeals/](https://www.reddit.com/r/usenet/wiki/providerdeals/)

Indexers: [https://www.reddit.com/r/usenet/wiki/indexers/](https://www.reddit.com/r/usenet/wiki/indexers/)

  

Pros and Cons list for Torrent vs UseNet
----------------------------------------

Torrent

**Pros**

**Cons**

Torrenting is free besides the VPN (optional but highly recommended depending on region)

torrents are tracked by your ISP and illegal in certain countries

May be able to find stuff you can't find on usenet

Slow Downloads

Huge variety of content

Requires you to share or reseed

Easy to learn and setup

Completion is iffy with older and less sought after files

No retention limit, as longs as people are seeding the files

Quality of files is typically not as good as usenet

Better chance of Internet provider banning/blocking you or busting you for downloads (if ou don�t use VPN)

UseNet

**Pros**

**Cons**

Always the fastest speed the server can provide (usually enough to max out your ISP)

Cost money (but you can find some good deals)

No VPN needed as you get SSL encryption with most servers included

A little tricky to setup but using this guide will hopefully help

No seeding, so you can turn your computer off & save electricity and not waste bandwidth

Difficult to understand at first, but hopefully this guide will help!

High quality files

Files can be removed for copyright

You can find almost anything popular, even if old. 10-15 years is how long data is kept on the servers typically (growing daily) but anybody can upload older files.

Rare/obscure stuff can be hard to find

### Why are people talking about Linux ISOs?

To bypass the rule of not talking about piracy in r/usenet, people started calling media (movies, TV shows etc) for linux ISOs (since linux is free and open source). It�s really just an ongoing joke aswell as a method of bypassing this rule.

### What is the difference between providers and indexers, and what are their roles?

ELI5 (Explain Like I�m 5):

Let�s say a provider owns a forest of LAND, a forest in which many people have buried their favorite.. Linux ISO�s � for all to share. These buried items are magical in that when you unbury it, you get a copy of the item and the item stays buried in the same spot for others to find. There�s probably all kind of things buried all over the place, some are things you�d probably never want or need. You dig into one random spot and you find something! It�s an empty Coca Cola bottle� well that�s not great. I�m sure there are people out there who would want it, but you have zero interest int that bottle.

This makes you realize that you now a huge problem, you paid the provider to have access to the forest but you have no clue where anything you want is buried.

That�s where the indexer comes in. Indexers give you access to their treasure maps that show where stuff is buried. Now you can use your treasure map to find the things you want!

As you go along your path of unburying the stuff you want, you realize that their map isn�t perfect. Sometimes the thing you want is nowhere on their map. It is possible that the thing you want isn�t buried anywhere in the forest, but it is just as possible that this particular map doesn�t know where everything is buried, they just do the best they can to keep track of as many buried things as they can. That�s when you decide to get other indexers, I mean treasure maps. With multiple treasure maps of the same forest, you have a good chance of finding items that you want, because one map may have a location that the others are missing! So having multiple maps is great because you are likelier to know the location of anything you are looking for in the forest.

Bonus eli5: you notice indexer treasure maps are way bigger than the forest, they go out into the mountains and the desert and the plains, all just as good to bury stuff. Of course you only paid one provider access to the forest. If you want to have access to other lands you realize you have to find and pay the provider that owns the deserts, or the one that owns the mountains. Having multiple providers (with different backbones) gives you access to more land that has potential to have buried items in it. Some providers sell the access to the same forest(aka same backbone) because they pay the real forest owner for rights to also sell access to that forest. Buying access to that forest twice(two providers with same backbone) is a waste of money because you already have access from one, so you want to make sure that if you get multiple providers, they give you access to different backbones, err, I mean lands.

\-Ericstern, rediit. [https://www.reddit.com/r/usenet/comments/1641vak/comment/jy7gsj7/?utm\_source=share&utm\_medium=web3x&utm\_name=web3xcss&utm\_term=1&utm\_content=share\_button](https://www.reddit.com/r/usenet/comments/1641vak/comment/jy7gsj7/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)

A lot of the provider deals, especially on black Friday, are for 15 months instead of 12. Is this a trick to make you renew when it�s not a sale?
-------------------------------------------------------------------------------------------------------------------------------------------------

Well, not really. Almost all the popular providers and indexers let you stack time, so either you can buy in multiple bulks now to get 2x15, 3x15 or even 4x15 months of access. Or you can wait until next black Friday (or another deal opportunity) and stack more time.

But beware the process can be a little bit different for some providers. Some might for example only stack on the same plan, so you can�t upgrade your account. It is always a good idea to research a little bit beforehand and maybe even contact either support on their website or a representative on reddit. They are usually really helpful with this kind of things.

  

Okay, I�m convinced. But what provider should I go for, and should I do an unlimited monthly/yearly plan or a block account?
----------------------------------------------------------------------------------------------------------------------------

Check out this reddit post: [https://www.reddit.com/r/usenet/comments/f215ko/a\_new\_users\_guide\_to\_picking\_providers\_questions/](https://www.reddit.com/r/usenet/comments/f215ko/a_new_users_guide_to_picking_providers_questions/)

My recommendation would probably to go for [Eweka](https://www.eweka.nl/en) has your main provider with unlimited access if you are in the EU, or [Newshosting](https://www.newshosting.com/) if you are in the US. Try to get a deal for $2.50 or $3.00 a month. Then if you wish you can also do block accounts on different backbones like Usenet Express or Abavia. Depending on usage you could also do something as crazy as myself and go for 2 unlimited accounts. I have 1 on [Eweka](https://www.eweka.nl/en)(Omicron) and 1 on [Frugal Usenet](https://frugalusenet.com/) (Usenet.Farm and NetNews multi-backbone).

To check which providers use which backbone, take a look at this map (updated as of November 2024) [https://cdn.rexum.space/usenet/14t2.svg](https://cdn.rexum.space/usenet/14t2.svg).

The important thing is the big main block at the top. The branches from that don�t really matter. E.g [Eweka](https://www.eweka.nl/en), Base IP, and HW Media are all on Omicron and will therefore yield the same results.

To find some good deals on providers, check out the reddit wiki here: [https://www.reddit.com/r/usenet/wiki/providerdeals/](https://www.reddit.com/r/usenet/wiki/providerdeals/)

Okay cool, what about indexer?
------------------------------

For indexers, you should have multiple for the best possible results and experience. The most popular (and best ones) are [NZBGeek](https://nzbgeek.info/), [DrunkenSlug](https://drunkenslug.com/), [NZB.su](https://nzb.su) and [NinjaCentral](https://ninjacentral.co.za). Note that both [DrunkenSlug](https://drunkenslug.com/) and [NinjaCentral](https://ninjacentral.co.za) are semi-private indexers which either requires you to register when they have open registration a few times a year or be invited by another user.

Some indexers also provide lifetime access, while others are a yearly sum you pay. Some offer both as different plans. Note that lifetime refers to the lifetime of the service, and it is not guaranteed to last your lifetime. It might shut down tomorrow, or in 50 years. Who really knows?

Here are a few good indexers I would recommend, in no particular order:

**Lifetime Membership:**

**Indexer**

**Registrations**

**Membership fee**

**Crypto**

**Account Limits**

[NZBGeek](https://nzbgeek.info/)

Open

$80

Yes

Unlimited

[Usenet-Crawler](https://www.usenet-crawler.com/)

Open

$20

Yes

1000 NZBs, 10,000 API hits/day

[AltHUB](https://althub.co.za/)

Open

$55

Yes

Unlimited

[NzbPlanet](https://nzbplanet.net/)

Open

�40

Yes

Unlimited NZBs, 20,000 API hits/day

**Yearly Membership:**

**Indexer**

**Registrations**

**Membership fee**

**Crypto**

**Account Limits**

[abNZB](https://abnzb.com/)

Open

$15 / $25

Yes

750 NZBs, 2,500 API hits/day / 2,500 NZBs, 10,000 Api hits/day

[AltHub](https://althub.co.za/)

Open

$10/yr / $25/3yrs / $40/5yrs

Yes

Unlimited

[DrunkenSlug](https://drunkenslug.com/)

Invite Only

�15 / �25

Yes

100 NZBs, 100 API hits/day, Unlimited

[NinjaCentral](https://ninjacentral.co.za/)

Closed

$15 / $25 / $150

Yes

Dan 0: 350 NZBs , 2000 API hits/day / Purplex: 900 NZBs , 3000 API hits/day / UNLIM: 10000 NZBs , 20000 API hits/day

[NzbPlanet](https://nzbplanet.net/)

Open

$12 / $24

Yes

VIP: Unlim NZBs, 2000 API hits/day / Platinum: Unlim NZBs, 20000 API hits/day

[NZBGeek](https://nzbgeek.info/)

Open

6U$/6Months / $12/yr / $18/2yrs / $40/5yrs

Yes

Unlimited

[nzb.su](https://nzb.su/)

Open

$15/yr / $28/2yrs / $42/3yrs

Yes

VIP: 600 NZBs, 5000 API hits/day

**Free Membership**

**Indexer**

Registration

Free Account Limits

Crypto

Upgradable through donations?

[AnimeTosho](https://animetosho.org/)

Open

Not that I�m aware of

No

No

[DrunkenSlug](https://drunkenslug.com/)

Invite-only

5 NZBs, 25 API hits/day

Yes

Yes

[BinSearch](https://www.binsearch.info/)

Open

Not that I�m aware

No

No

[DigitalCarnage](https://digitalcarnage.info/)

Open

10 NZBs, 10 API hits/day

Yes

Yes

[AltHub](https://althub.co.za/)

Open

25 NZBs, 100 API hits/day

Yes

Yes

You can check out the whole matrix/list of indexers on the reddit wiki here: [https://www.reddit.com/r/usenet/wiki/indexers/](https://www.reddit.com/r/usenet/wiki/indexers/)

Wow, that�s a lot of choices. What do you recommend for a beginner?
-------------------------------------------------------------------

If you feel overwhelmed and don�t know where to start, I would go for a membership on [eweka](https://www.eweka.nl/) as your provider (on sale of course, as there are always sales. Check the wiki). For indexer I would recommend [NZBGeek](https://nzbgeek.info/). Check also if [DrunkenSlug](https://drunkenslug.com/) and [NinjaCentral](https://ninjacentral.co.za/) have open registration, as they are 2 of the most powerful indexers. If you just want something cheap, [usenet\-crawler](https://usenet-crawler.com/) wouldn�t be bad either.

If you want to really do something crazy, you could even have multiple indexers to find even more stuff. And add block accounts on UsenetExpress or Abavia to fill in Ewekas gaps. But this can also come at a later point in time.

  

What is a newsreader?
---------------------

The newsreader is the term used for the downloader. You need it to read the xml files (news), download them, and then to reconstruct the original file. Before, in the old days, a lot of the good ones cost money. Today, the 2 most popular ones are free; Sabnzbd and NZBGet. NZBGet is very on and off with support, and at the time of writing it haven�t had any updates in over 3 years. Meanwhile Sabnzbd got an update yesterday. So, I would personally choose Sabnzbd, but I guess that�s personal preference.

  

Now I have a provider and an indexer, how to set it up with the \*arrs?
-----------------------------------------------------------------------

It is actually very simple to set it up with the \*arrs. If you wish to keep your VPN (good idea if you still have time on it for more privacy) you don�t have to do anything on the yaml file except add a newsreader of choice. Then you just add this portion to your yaml:

  sabnzbd:

    image: lscr.io/linuxserver/sabnzbd:latest

    container\_name: sabnzbd

    network\_mode: service:gluetun

    environment:

      - PUID=<your UID>

      - PGID=<your GID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/sabnzbd/config:/config

      \- /volume1/Media:/Media

    restart: unless-stopped

    security\_opt:

      - no-new-privileges:true

    depends\_on:

      gluetun:

        condition: service\_healthy

Also be sure to add port 8080:8080 in GlueTun.

  

If you don�t want to use a VPN, either because you want to use that money on a better provider, or an additional indexer or something else, then you will have to remove the whole GlueTun container. In addition, you would need to change the network mode on all containers from service:gluetun to host, or another bridge you might have. Then you would need to add all the ports required by each service. This is an example:

  sabnzbd:

    image: lscr.io/linuxserver/sabnzbd:latest

    container\_name: sabnzbd

    network\_mode: host

    environment:

      - PUID=<your UID>

      - PGID=<your UID>

      - TZ=Europe/Oslo

    volumes:

      - /volume1/docker/arr\-stack/sabnzbd/config:/config

      - /volume1/Media:/Media

    ports:

      - 8080:8080/tcp

    restart: unless-stopped

    security\_opt:

      - no-new-privileges:true

    depends\_on:

      gluetun:

        condition: service\_healthy

Personally, I also prefer to replace prowlarr with nzbhydra2. This is 100% optional and personal preference. But I do recommend using either one of these 2 instead of adding the indexers directly to Sonarr and Radarr, especially with UseNet. That is because they provide good stats that can help you with your financial decisions. If you see an indexer is nearly never used, why bother renewing it next year?

  

For NZBHydra 2, you can add this to your yaml, and make the appropriate modifications:

nzbhydra2:

    image: lscr.io/linuxserver/nzbhydra2:latest

    container\_name: nzbhydra2

    network\_mode: host

    environment:

      - PUID=<your UID>

      - PGID=<your GID>

      - TZ=Europe/Oslo

    ports:

      - 5076:5076/tcp

    volumes:

      - /volume1/docker/arr\-stack/nzbhydra2:/config

      - /volume1/Media/Usenet

    restart: unless-stopped

Then you will also have to create a nzbhydra2 folder inside your arr\-stack folder (in docker shared volume). Now we can start to configure our apps.

  

Configuring the apps
--------------------

### Sabnzbd

Open your web browser and navigate to <nas-ip\>:8080. You will have to create an account for login credentials. When you have signed in, you will need to click the gear icon at the top right.

![Et bilde som inneholder tekst, programvare, Multimedieprogramvare, skjermbilde
Automatisk generert beskrivelse](media-filer/image153.jpg)

Then navigate to the �Servers� tab. Click add server. Then fill in your information, you can find everything on your provider�s website. Also select the priority you want, you should always have your main unlimited account set to 0 or 1 as the highest priority, then block with a lower priority (higher number). That way it only use the blocks if the main provider does not have the complete file. And always, always, always have SSL enable, if not your ISP can and will send you warning for copyright infringement. If you click on �Advanced Settings�, you can even double check the SSL port is correct.

![Et bilde som inneholder skjermbilde, tekst, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image155.png)

When that is done, you can click �Test Server� and if it works great, if not double check your information is correct.

  

### NZBHydra2

I am using NZBHydra 2, but Prowlarr will be almost identical. You have already set up torrent trackers on Prowlarr, so this will be no problem for you. But this is how to setup NZBHydra2:

1.      Navigate to <nas-ip\>:5076 on your browser.

2.      Select config

![Et bilde som inneholder tekst, skjermbilde, Font, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image157.png)

3.      Go to the indexers tab and click on �Add Indexer�

4.      Select �Choose from preset�. If you can�t find your indexer, then select �Add custom newznab indexer�

5.      For this example, I will add DrunkenSlug. Fill in your information. All should be on your provider website:

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image159.png)

If you don�t have an API or download limit, and your VIP never expires you can leave these fields blank.

6.      Click �Submit�

**7.**      **REMEMBER TO CLICK �SAVE�**

NZBHydra makes it very easy to connect it to the \*arrs. You can do it manually, like with Prowlarr, but you can also just click on �Configure NZBhydra in�� next to the save button

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image160.png)

Select Lidarr, Sonarr v3, Radarr v3 or Readarr. Normal Sonarr and Radarr are outdated and not used anymore. Then you just fill in your information.

![Et bilde som inneholder tekst, skjermbilde, programvare, Multimedieprogramvare
Automatisk generert beskrivelse](media-filer/image162.png)

That�s it! Now you can download with Radarr and Sonarr using UseNet! You can also do it manually. Sometimes Radarr and Sonarr can�t find everything on the indexer. Then it can be good to browse yourself.

You could do this by going to each indexer and searching, but with NZBHydra you can search ALL your indexers at the same time. Then just select the one(s) you wish to download and select �Results as zip�. You can also download each file individually by clicking the download button to the right of each file. Then just go to Sabnzbd, click the + button at the top right and upload either your zip file or nzb file. If you select category movies or series (or whatever you have configured with Sonarr and Radarr) they will automatically also get picked up and imported by the respective apps.

Now, just lean back and enjoy your experience with UseNet!

Thanks for reading my guide. I hope this was helpful to you. If it was, be sure to let me know with a comment, or upvote the reddit post! You can also star the Github project or send me a DM letting me know how awesome this guide was 😊

  

Sources
=======

Marius Hosting have a lot of great guides on how to setup different things on Synology:

[https://mariushosting.com/](https://mariushosting.com/)

DrFrankenstein�s Tech Stuff also has a lot of useful information on a bunch of subjects within the synology ecosystem:

[https://drfrankenstein.co.uk/](https://drfrankenstein.co.uk/)

TRaSH Guides. The BEST source for configuring Radarr and Sonarr:

[https://trash-guides.info/](https://trash-guides.info/)

Radarrs official docs:

[https://github.com/Radarr/Radarr](https://github.com/Radarr/Radarr)

Sonarrs official docs:

[https://github.com/sonarr/sonarr](https://github.com/sonarr/sonarr)

Lidarrs official docs:

[https://github.com/lidarr/lidarr](https://github.com/lidarr/lidarr)

Overseerrs official docs:

[https://github.com/sct/overseerr](https://github.com/sct/overseerr)

Requestrrs official docs:

[https://github.com/darkalfx/requestrr](https://github.com/darkalfx/requestrr)

GlueTUNs official docs:

[https://github.com/qdm12/gluetun-wiki](https://github.com/qdm12/gluetun-wiki)

Awesome -arrs wiki:

[https://github.com/Ravencentric/awesome-arr](https://github.com/Ravencentric/awesome-arr)

Wikipedia, Usenet:

[https://en.wikipedia.org/wiki/Usenet](https://en.wikipedia.org/wiki/Usenet)

NZBGet GitHub Project:

[https://github.com/nzbget/nzbget](https://github.com/nzbget/nzbget)

Sabnzbd GitHub Project:

[https://github.com/sabnzbd/sabnzbd](https://github.com/sabnzbd/sabnzbd)

The amazing UseNet subreddit. Lots of helpful people and helpful articles:

[https://www.reddit.com/r/usenet](https://www.reddit.com/r/usenet)