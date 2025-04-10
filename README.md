# CBT312
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 312 is from Lionel Dyck in Austin, Texas and contains     *   FILE 312
//*           quite a few ISPF interface packages, and other        *   FILE 312
//*           stuff.                                                *   FILE 312
//*                                                                 *   FILE 312
//*           The member list probably more accurately reflects     *   FILE 312
//*           the contents of this file, than does the description  *   FILE 312
//*           of some details, below.  This file is constantly      *   FILE 312
//*           being revised.  For reference, please see Lionel's    *   FILE 312
//*           web site at:   http://github.com/lbdyck               *   FILE 312
//*                                                                 *   FILE 312
//*           email:  lbdyck@gmail.com                              *   FILE 312
//*                                                                 *   FILE 312
//*    Lionel Dyck's large collection of utilities has now been     *   FILE 312
//*    divided between Files 312, 313, 314, and 969.  All member    *   FILE 312
//*    names beginning with A-R are on File 312.  Names beginning   *   FILE 312
//*    with S-TS are on File 313.  Names from TX-Z are on File      *   FILE 312
//*    314.  File 969 contains the PDSEGEN ISPF application to      *   FILE 312
//*    exploit the capabilities of using PDSE Version 2 member      *   FILE 312
//*    generations.                                                 *   FILE 312
//*                                                                 *   FILE 312
//*    These four files contain quite a few separate utility        *   FILE 312
//*    packages which are unrelated to each other.  You can tell    *   FILE 312
//*    which members of these files belong to the same utility      *   FILE 312
//*    package, by the similarities in their member names.          *   FILE 312
//*                                                                 *   FILE 312
//*    Some utility packages will have several member names         *   FILE 312
//*    associated with them.  But these should all be similar       *   FILE 312
//*    to each other, letting you know that they belong to the      *   FILE 312
//*    same utility package.  You can see this, by looking at       *   FILE 312
//*    the member list shown below, so you can get the idea         *   FILE 312
//*    about how this packaging arrangement works.                  *   FILE 312
//*                                                                 *   FILE 312
//*    Documentation files which are in WORD format, or PDF         *   FILE 312
//*    format, have been included to make the use of the package    *   FILE 312
//*    associated with the doc, easier.  Usually a doc file in      *   FILE 312
//*    FB-80 EBCDIC text, has been included too.  To use the        *   FILE 312
//*    WORD or PDF format documentation, you have to download the   *   FILE 312
//*    member in BINARY to a PC, and look at the resulting file     *   FILE 312
//*    on the PC, using Microsoft WORD, or Adobe ACROBAT reader,    *   FILE 312
//*    respectively.                                                *   FILE 312
//*                                                                 *   FILE 312
//*       NAME       VER.MOD   LAST MODIFIED     SIZE   ID          *   FILE 312
//*       $DOC        01.06   2022/10/13 11:42     16 LBDYCK        *   FILE 312
//*       ADDCOMMA    01.00   2022/12/09 09:51     34 COMMA         *   FILE 312
//*       ALIGN       01.01   2019/12/31 06:41    216 ALIGN         *   FILE 312
//*       ALLOCGDG    01.00   2003/02/05 14:04    138 SYSLBD        *   FILE 312
//*       ALTLIBST    01.00   2022/01/31 09:33     66 ALTLIB        *   FILE 312
//*       BACKDIR     01.00   2017/07/11 14:14    359 LBD           *   FILE 312
//*       BISPFJCL    01.01   2016/11/16 10:18    526 SYSLBD        *   FILE 312
//*       BODY        01.00   2020/02/29 09:16    139 XMIT          *   FILE 312
//*       CAVXTR$     01.21   2003/06/02 08:27     77 SYSLBD        *   FILE 312
//*       CAVXTR$$    01.26   2010/05/21 01:24     92 SYSLBD        *   FILE 312
//*       CAVXTR#     01.26   2010/05/21 01:26   2080 PDF           *   FILE 312
//*       CAVXTR@     01.26   2010/05/21 01:26   2093 MSWORD        *   FILE 312
//*       CAVXTRT     01.27   2019/01/23 06:12   2725 CAV           *   FILE 312
//*       CHGSTR      01.00   2022/10/13 11:42     44 LBDYCK        *   FILE 312
//*       CHKIKJ      01.07   2017/06/15 12:28    977 LBD           *   FILE 312
//*       CHKLPALK    01.00   2016/11/23 06:51     90 SYSLBD        *   FILE 312
//*       CHKPDSE     01.01   2016/11/09 07:37     67 FILE312       *   FILE 312
//*       CLONE       01.00   2016/11/08 09:56    427 SYSLBD        *   FILE 312
//*       CMDS        01.00   2000/02/16 16:27    588 SYSLBD        *   FILE 312
//*       CMDSRPT     01.06   2016/03/17 07:47     74 SYSLBD        *   FILE 312
//*       CMDSRPTO    01.02   2016/03/02 14:50     43 SYSLBD        *   FILE 312
//*       CMT         01.14   2024/08/02 11:44   1319 LBDYCK        *   FILE 312
//*       COMPVTC$    01.01   2001/02/09 12:23     21 WSBG          *   FILE 312
//*       COMPVTOC    01.00   2001/02/09 12:23     58 SYSLBD        *   FILE 312
//*       CONCATIT    01.00   2020/08/23 09:08    554 SLBD          *   FILE 312
//*       CONS        01.06   2021/02/13 21:00     38 CONS          *   FILE 312
//*       COPYFB      01.02   2016/04/03 15:00     70 SYSLBD        *   FILE 312
//*       CSVEDIT     01.11   2008/04/15 11:10    542 SYSLBD        *   FILE 312
//*       CSVEDIT#    01.11   2008/04/15 11:12   2541 PDF           *   FILE 312
//*       CSVEDIT@    01.11   2008/04/15 11:12   1434 MSWORD        *   FILE 312
//*       CUTPASTE    01.00   1999/07/06 18:40   1326 SYSLBD        *   FILE 312
//*       DDLIST      01.00   2003/09/30 09:33   1607 SYSLBD        *   FILE 312
//*       DDLIST$     01.01   2003/09/29 07:29      6 SYSLBD        *   FILE 312
//*       DOALL       01.01   2016/11/09 07:44     56 FILE312       *   FILE 312
//*       DOTSO       01.01   2024/04/05 11:14     14 DOTSO         *   FILE 312
//*       DROPISPF    01.00   2018/12/06 07:18     28 DROPSPF       *   FILE 312
//*       DSFSADM     01.09   2024/01/30 08:52   1289 DSFSADM       *   FILE 312
//*       DSLIST      01.00   2000/02/15 21:40    106 SYSLBD        *   FILE 312
//*       DUMPMGMT    01.00   2001/09/25 16:49   1369 SYSLBD        *   FILE 312
//*       EDITMAC     01.01   2020/07/30 06:28    157 EDITMAC       *   FILE 312
//*       EDSL        01.99   2021/01/14 13:50   2903 SLBD          *   FILE 312
//*       EKKO        01.00   2016/11/05 13:57    413 CBTUSER       *   FILE 312
//*       EKKO$       01.10   2016/11/06 20:21     27 SBGOLOB       *   FILE 312
//*       EKKOH       01.00   2016/12/02 06:14     78 SBGOLOB       *   FILE 312
//*       EMAC        02.03   2021/08/25 09:44   1183 EMAC          *   FILE 312
//*       EXTISPF     01.00   2018/05/18 13:56    227 EXTISPF       *   FILE 312
//*       EZMENU      01.06   2025/03/26 12:36    873 EZMENU        *   FILE 312
//*       FASTPATH    01.08   2023/07/28 07:29   1326 FASTP         *   FILE 312
//*       FINDDDM     01.02   2013/10/28 11:21     93 MVSLBD1       *   FILE 312
//*       FINDDSN     01.04   2019/05/09 08:47     94 SLBD          *   FILE 312
//*       FIXBOOKP    01.00   2000/05/05 12:18    138 WSBG          *   FILE 312
//*       FIXKEYS     01.10   2024/03/18 07:52    852 FIXKEYS       *   FILE 312
//*       FIXKEYS$    01.03   2024/03/18 07:52     24 FIXKEYS       *   FILE 312
//*       FIXNL       01.01   2016/11/16 10:23     49 SYSLBD        *   FILE 312
//*       FTPB        02.33   2024/01/19 07:33   9761 FTPB          *   FILE 312
//*       FTPB$CHG    02.33   2024/01/19 07:34    361 FTPB          *   FILE 312
//*       FTPB#       02.24   2019/07/02 11:23   4146 PDF           *   FILE 312
//*       FTPB@       02.24   2019/07/02 11:23    692 MSWORD        *   FILE 312
//*       FTPFROMZ    01.00   2004/05/23 08:07   1131 SYSLBD        *   FILE 312
//*       FTPFROZC    01.00   2004/05/23 08:06     22 SYSLBD        *   FILE 312
//*       GENSUB      01.00   2002/02/19 10:39    188 SYSLBD        *   FILE 312
//*       GET         01.00   2000/02/16 16:49     88 SYSLBD        *   FILE 312
//*       GETIPLDT    01.03   2024/08/02 09:38     94 LBDYCK        *   FILE 312
//*       HIDELINE    01.00   2016/04/04 11:55     46 SYSLBD        *   FILE 312
//*       IDLIST      01.00   2016/11/08 10:35     62 SYSLBD        *   FILE 312
//*       IEBPDSE     01.12   2017/11/01 06:07    591 LBD           *   FILE 312
//*       IFTHENEL    01.00   2017/04/24 09:07     61 LBDYCK        *   FILE 312
//*       INEWS       01.09   2017/02/15 13:54   2691 SYSLBD        *   FILE 312
//*       IPLTCHK     01.00   2018/09/15 10:30    109 IPLTCHK       *   FILE 312
//*       IPLTCHK$    01.02   2018/09/15 11:59     40 IPLTCHK       *   FILE 312
//*       ISPFCMDS    01.01   2003/05/23 11:13    388 SYSLBD        *   FILE 312
//*       ISPFDEMO    01.00   2021/04/27 05:12    764 DEMO          *   FILE 312
//*       ISPFLLV     01.02   2022/05/29 13:37    672 ISPFLLV       *   FILE 312
//*       ISPFPRO$    01.00   2000/02/28 20:46    101 SYSLBD        *   FILE 312
//*       ISPFPROD    01.00   2000/08/21 17:40    429 SYSLBD        *   FILE 312
//*       LDAPMAI$    01.00   2000/11/22 10:54      6 WSBG          *   FILE 312
//*       LDAPMAIL    01.01   2003/08/27 10:31    344 SYSLBD        *   FILE 312
//*       LDAPMCHG    01.01   2003/08/26 14:45      6 SYSLBD        *   FILE 312
//*       LOADISPF    01.05   2019/01/09 06:55    324 ISPF          *   FILE 312
//*       LOG         01.00   2016/11/08 01:09    304 SYSLBD        *   FILE 312
//*       LOGARCH     01.01   2016/11/16 10:28    183 SYSLBD        *   FILE 312
//*       LOGIT       01.00   2004/04/20 11:45    458 LBDYCK        *   FILE 312
//*       LOGIT$      01.00   2004/04/20 11:45     84 LBDYCK        *   FILE 312
//*       LOGITCHG    01.00   2004/04/20 11:45     22 LBDYCK        *   FILE 312
//*       LOWER       01.01   2016/12/21 09:21     15 SYSLBD        *   FILE 312
//*       LPREDIT     01.01   2014/03/20 22:46     26 LBDYCK        *   FILE 312
//*       LPRPRINT    01.03   2018/02/14 07:48   1341 PRINT         *   FILE 312
//*       LPRPROLD    01.00   2014/03/21 10:56    421 LBDYCK        *   FILE 312
//*       LSTPRC      01.53   2008/11/01 22:12    817 SBGOLOB       *   FILE 312
//*       LSTPRC$     01.02   2018/02/16 14:32     19 SBGOLOB       *   FILE 312
//*       LSTPROC     03.04   2023/04/14 12:38    992 LSTPROC       *   FILE 312
//*       LSTPROC$    01.03   2016/04/19 14:16     10 SBGOLOB       *   FILE 312
//*       LSTPROC#    01.01   2016/11/16 10:30     24 LSTPROC       *   FILE 312
//*       LSTPROC@    01.00   2000/10/25 10:36     29 WSBG          *   FILE 312
//*       LSTPROC3    03.04   2018/09/27 14:24    812 FORJES3       *   FILE 312
//*       MGEN        01.01   2016/11/16 10:31     24 SYSLBD        *   FILE 312
//*       NETRC       01.02   2021/01/26 00:58    629 NETRC         *   FILE 312
//*       OMVSCMD     01.05   2024/01/03 07:52    472 OMVSCMD       *   FILE 312
//*       OMVSCMDS    01.11   2025/03/28 14:55    670 OMVSCMDS      *   FILE 312
//*       OMVSCOPY    02.18   2018/08/10 06:51   2595 OMVS          *   FILE 312
//*       OMVSLOG     01.02   2016/11/16 10:34    399 SYSLBD        *   FILE 312
//*       OMVSMAN     02.07   2025/02/21 10:39   1064 OMVSMAN       *   FILE 312
//*       OMVSPAX     01.02   2020/09/17 06:57   1185 PAX           *   FILE 312
//*       OMVSSEL     01.04   2018/08/16 07:37    869 OMVS          *   FILE 312
//*       OMVSTRY     01.00   2025/03/27 09:03     64 OMVSTRY       *   FILE 312
//*       ONCALL      01.00   2003/12/11 08:04    625 SYSLBD        *   FILE 312
//*       ONCALL#     01.00   2003/12/02 18:23     11 SYSLBD        *   FILE 312
//*       ONLY        01.07   2019/12/24 04:10    551 ONLY          *   FILE 312
//*       PACK        01.00   2016/04/17 18:21    660 TRSMAIN       *   FILE 312
//*       PDS2PDSE    01.03   2021/05/31 12:55    798 P2PE          *   FILE 312
//*       PDS2SEQ     01.02   2016/07/03 10:19    154 WSYNGUD       *   FILE 312
//*       PDS2SEQ$    01.01   2016/11/07 23:29     21 SYSLBD        *   FILE 312
//*       PLPISPF     01.51   2020/02/18 10:16   4364 XMIT          *   FILE 312
//*       PLPISPF$    01.49   2020/02/18 10:17    217 PLP           *   FILE 312
//*       PLPISPF#    01.29   2016/04/03 18:42   3369 PDF           *   FILE 312
//*       PLPISPF@    01.29   2016/04/03 18:42   1172 MSWORD        *   FILE 312
//*       PNS         01.00   2016/12/08 10:51     93 SYSLBD        *   FILE 312
//*       PRMCK       02.08   2021/10/01 06:59   2781 PRMCK         *   FILE 312
//*       PRMCK$      01.09   2018/09/13 05:40     50 PRMCK         *   FILE 312
//*       PRMCK#      01.00   1999/11/11 11:32      9 SYSLBD        *   FILE 312
//*       PSPRINT     01.02   2015/04/30 16:13    567 LBDYCK        *   FILE 312
//*       PSPRINTO    01.00   2014/03/21 11:02    553 LBDYCK        *   FILE 312
//*       QTAB        03.02   2023/04/03 12:58    787 LBDYCK        *   FILE 312
//*       RANDSTR     01.02   2018/02/27 06:16    151 LBD           *   FILE 312
//*       RELPDSE     01.05   2023/01/04 08:11    135 RELPDSE       *   FILE 312
//*       REXXDOC     01.00   2001/01/05 11:31    265 SYSLBD        *   FILE 312
//*       REXXER      01.10   2020/10/28 05:15    408 SLBD          *   FILE 312
//*       REXXFORM    01.04   2017/04/26 09:52    515 LBD           *   FILE 312
//*       REXXTRY     01.00   2000/11/08 18:46    187 REXXTRY       *   FILE 312
//*       REXXTRY$    01.00   2000/11/08 18:46     78 REXXTRY       *   FILE 312
//*       REXXTRY#    01.00   2000/11/08 18:56      9 WSBG          *   FILE 312
//*       REXXTRY@    01.00   2000/11/08 18:46     35 REXXTRY       *   FILE 312
//*       REXXTRYA    01.00   2000/12/26 17:20     77 REXXTRY       *   FILE 312
//*       REXXWAIT    01.00   2000/02/16 16:59    207 SBGOLOB       *   FILE 312
//*       RUNC        06.01   2020/07/30 06:27   8567 RUNC          *   FILE 312
//*       RUNCPP      01.00   2016/11/06 21:42   3159 POWERPT       *   FILE 312
//*                                                                 *   FILE 312
//*       ** Note: WORD members may require replying YES to         *   FILE 312
//*                Microsoft Word document recovery to open.        *   FILE 312
//*                                                                 *   FILE 312
//*  Member $DOC - basic information                                *   FILE 312
//*                                                                 *   FILE 312
//*  Member ALIGN - added 12/31/19                                  *   FILE 312
//*                                                                 *   FILE 312
//*         ISPF Edit Macro to Align the text on the                *   FILE 312
//*         specified line or lines.                                *   FILE 312
//*                                                                 *   FILE 312
//*          Options:                                               *   FILE 312
//*          ? display help                                         *   FILE 312
//*          C ll - strip and center                                *   FILE 312
//*          F ll - flow text to line length(ll)                    *   FILE 312
//*          L - strip and left justify                             *   FILE 312
//*          R - strip and right justify                            *   FILE 312
//*          V - strip and reverse text                             *   FILE 312
//*                                                                 *   FILE 312
//*          Optional for C is ll for line length                   *   FILE 312
//*          e.g. ALIGN C 65                                        *   FILE 312
//*               To align center for a width of 65                 *   FILE 312
//*                                                                 *   FILE 312
//*          Select row/rows using C/CC                             *   FILE 312
//*                                                                 *   FILE 312
//*  Member ALTLIBST - added 2022/01/30                             *   FILE 312
//*                                                                 *   FILE 312
//*      Nice display of active ALTLIB allocations with dsnames.    *   FILE 312
//*                                                                 *   FILE 312
//*  Member ADDCOMMA - added 2022/12/09                             *   FILE 312
//*                                                                 *   FILE 312
//*      Sample REXX to add commas to a number                      *   FILE 312
//*         - 999999 to 999,999                                     *   FILE 312
//*                                                                 *   FILE 312
//*  Member BACKDIR - added 07/11/17                                *   FILE 312
//*                                                                 *   FILE 312
//*     OMVS utility written in rexx to backup complete directories *   FILE 312
//*                                                                 *   FILE 312
//*  Member BODY    - added 02/29/20                                *   FILE 312
//*                                                                 *   FILE 312
//*     ISPF Edit macro to report on the size of the BODY section   *   FILE 312
//*     of a panel. Also recommends window size and addpop parms.   *   FILE 312
//*                                                                 *   FILE 312
//*  Member CAVXTRT                                                 *   FILE 312
//*         - Updated 1/23/19 for CAView 14.x                       *   FILE 312
//*                                                                 *   FILE 312
//*     This dialog is intended as a more user friendly interface   *   FILE 312
//*     to the reports. The options available with this dialog      *   FILE 312
//*     are:                                                        *   FILE 312
//*                                                                 *   FILE 312
//*             - Broswe a report (using ISPF Browse)               *   FILE 312
//*             - View a report (using ISPF View)                   *   FILE 312
//*             - Copy a report to a dataset                        *   FILE 312
//*             - Mail a report (using XMITIP)                      *   FILE 312
//*             - Print a report                                    *   FILE 312
//*             - Transfer a report to a workstation                *   FILE 312
//*             - Load a report from CA-View tape to CA-View disk   *   FILE 312
//*                                                                 *   FILE 312
//*     This code has been tested on OS/390 2.10 and z/OS 1.9       *   FILE 312
//*     with CA-View and CA-View 11.0. It is slightly (does a       *   FILE 312
//*     dynamic lookup) dependent upon the report format            *   FILE 312
//*     generated by SARBCH with the /LIST statement If this        *   FILE 312
//*     report format changes then the code which parses the        *   FILE 312
//*     report will have to be changed.                             *   FILE 312
//*                                                                 *   FILE 312
//*  Member CHGSTR (added 10/13/2022)                               *   FILE 312
//*                                                                 *   FILE 312
//*     CHGSTR is a simple rexx function for use on z/OS that       *   FILE 312
//*     provides most of the capabilities of the ANSI Standard      *   FILE 312
//*     REXX CHANGESTR function.                                    *   FILE 312
//*                                                                 *   FILE 312
//*  Member CHKIKJ (update 06/15/2017)                              *   FILE 312
//*                                                                 *   FILE 312
//*     CHKIKJ is a quick/dirty ispf dialog to compare the ibm      *   FILE 312
//*     samplib version of ikjtso00 to what is actually running     *   FILE 312
//*     on the active lpar.                                         *   FILE 312
//*                                                                 *   FILE 312
//*     TSO Transmit format member (so receive it).                 *   FILE 312
//*                                                                 *   FILE 312
//*  Member CHKLPALK                                                *   FILE 312
//*                                                                 *   FILE 312
//*     REXX exec to check all LPALIST and LINKLIST datasets for    *   FILE 312
//*     extents and report on same.                                 *   FILE 312
//*                                                                 *   FILE 312
//*  Member CMDS                                                    *   FILE 312
//*                                                                 *   FILE 312
//*     This data set contains an ISPF Dialog that simplifies the   *   FILE 312
//*     processing of the ISPF command tables.                      *   FILE 312
//*                                                                 *   FILE 312
//*  Member CMT    (updated 2024-08-02)                             *   FILE 312
//*                                                                 *   FILE 312
//*     ISPF Edit command (macro) to easily insert comments into    *   FILE 312
//*     source code using the target language correct syntax.       *   FILE 312
//*                                                                 *   FILE 312
//*  Member CONCATIT - added 8/23/2020                              *   FILE 312
//*                                                                 *   FILE 312
//*      ALLOCADD and DEALLOC are a combination of REXX exec's      *   FILE 312
//*      that provide the ability to add a dataset(s), or remove    *   FILE 312
//*      a dataset from an existing DD allocation.                  *   FILE 312
//*                                                                 *   FILE 312
//*      CONCATIT combines ALLOCADD and DEALLOC with a List option  *   FILE 312
//*      to provide a single exec instead of multiple.              *   FILE 312
//*                                                                 *   FILE 312
//*  Member CSVEDIT                                                 *   FILE 312
//*                                                                 *   FILE 312
//*     CSVEDIT - an ISPF Edit Macro designed to convert the        *   FILE 312
//*     current EDIT data set into a comma separated value data     *   FILE 312
//*     set which can then be imported into a spreadsheet or        *   FILE 312
//*     database.                                                   *   FILE 312
//*                                                                 *   FILE 312
//*  Member CUTPASTE - This member is in TSO XMIT format.           *   FILE 312
//*                                                                 *   FILE 312
//*     This member contains 2 REXX execs, CUT and PASTE,           *   FILE 312
//*     with ISPF panels that go together with them. **Ancient**    *   FILE 312
//*                                                                 *   FILE 312
//*  Member DOTSO (added 04/05/2024)                                *   FILE 312
//*                                                                 *   FILE 312
//*     Simple shell script for use on OMVS to execute a TSO        *   FILE 312
//*     command using a pre-defined load library as a STEPLIB.      *   FILE 312
//*     Requires minimal customization after adding to a directory  *   FILE 312
//*     in your PATH.                                               *   FILE 312
//*                                                                 *   FILE 312
//*  Member DROPISPF (added 12/06/2018)                             *   FILE 312
//*                                                                 *   FILE 312
//*     Companion to LOADISPF (thanks to John Kalinich)             *   FILE 312
//*                                                                 *   FILE 312
//*  Member DSFSADM (updated 01/30/2024)                            *   FILE 312
//*                                                                 *   FILE 312
//*     A simple ISPF menu dialog with 3 entry points:              *   FILE 312
//*           A - Administration (z/OS commands and dsadm commands) *   FILE 312
//*           D - dsadm commands for admin                          *   FILE 312
//*           U - user dsadm commands                               *   FILE 312
//*                                                                 *   FILE 312
//*     DSFS, or Data Set File System, provides OMVS shell users    *   FILE 312
//*     with Unix-like access to z/OS datasets (ps, pds, pdse).     *   FILE 312
//*                                                                 *   FILE 312
//*     This dialog helps those who administer DSFS to find which   *   FILE 312
//*     command to use, and helps them issue it, for something they *   FILE 312
//*     probably won't be doing frequently.                         *   FILE 312
//*                                                                 *   FILE 312
//*     See the excellent IBM DSFS publications for more details    *   FILE 312
//*     and specifics on the commands.                              *   FILE 312
//*                                                                 *   FILE 312
//*  Member EDITMAC (added 07/30/2020)                              *   FILE 312
//*                                                                 *   FILE 312
//*        Execute an inline ISPF Edit macro                        *   FILE 312
//*                                                                 *   FILE 312
//*  Member EDSL (updated 12/09/2020)                               *   FILE 312
//*                                                                 *   FILE 312
//*        ISPF Enhanced Data Set List. Works with Personal         *   FILE 312
//*        Data Set Lists (DSList, ISPF 3.4) and more.              *   FILE 312
//*                                                                 *   FILE 312
//*  Member EMAC (update 8/25/2021)                                 *   FILE 312
//*                                                                 *   FILE 312
//*        ISPF Edit Macro (command) to display a selection         *   FILE 312
//*        list of edit macros to the user from which the user      *   FILE 312
//*        can select to execute the command or display any help.   *   FILE 312
//*        Cursor placement and/or row selection(s) supported.      *   FILE 312
//*                                                                 *   FILE 312
//*        An excellent example of a scrollable data entry field    *   FILE 312
//*        on the popup for macro parms (thanks John K.).           *   FILE 312
//*                                                                 *   FILE 312
//*        The tutorial panel and parm prompt popup panels show     *   FILE 312
//*        the PF Keys that are defined for Left/Right/ZEXPand.     *   FILE 312
//*                                                                 *   FILE 312
//*        Only works under ISPF Edit/View and will display its     *   FILE 312
//*        tutorial if called otherwise.                            *   FILE 312
//*                                                                 *   FILE 312
//*  Member EXTISPF  - added 05/18/2018                             *   FILE 312
//*                                                                 *   FILE 312
//*        Can be used to extract the embedded ISPF elements        *   FILE 312
//*        from the exec's where I use the LOADISPF process.        *   FILE 312
//*                                                                 *   FILE 312
//*  Member EZMENU   - updated 2025 Mar 26                          *   FILE 312
//*                                                                 *   FILE 312
//*        A *new* simple way to create an ISPF Menu by using       *   FILE 312
//*        a easy to create and manage set of records. No more      *   FILE 312
//*        ISPF Panel coding.                                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member FASTPATH - updated 7/28/2322                            *   FILE 312
//*        - new packaging and enhancements                         *   FILE 312
//*                                                                 *   FILE 312
//*        Display a selection list of all Selectable               *   FILE 312
//*        commands in the ISPCMDS ISPF Command Table               *   FILE 312
//*        and in the System and User command tables                *   FILE 312
//*        along with the commands in the current application       *   FILE 312
//*        command table.  This command will:                       *   FILE 312
//*                                                                 *   FILE 312
//*        1.  Provide the user with information on                 *   FILE 312
//*            fast path commands available.                        *   FILE 312
//*        2.  Simplify access to fast path commands.               *   FILE 312
//*        3.  Provide a pseudo-menu to ISPF command                *   FILE 312
//*            functions.                                           *   FILE 312
//*        4.  If a tutorial panel exists for the command           *   FILE 312
//*            of the format $ followed by the first 7              *   FILE 312
//*            characters of the command name, it will be           *   FILE 312
//*            displayed if the user selects the command            *   FILE 312
//*            with 'H' or via PF1(Help) on the pop-up              *   FILE 312
//*            menu if the command has options.                     *   FILE 312
//*        5.  Generate a Report of all commands.                   *   FILE 312
//*                                                                 *   FILE 312
//*  Member FINDDDM                                                 *   FILE 312
//*         - added 5/9/19                                          *   FILE 312
//*                                                                 *   FILE 312
//*   Function: Find specified member in the specified DDname       *   FILE 312
//*             concatenation.                                      *   FILE 312
//*                                                                 *   FILE 312
//*   Usage:    called from a rexx or clist                         *   FILE 312
//*                                                                 *   FILE 312
//*             library = findddm()                                 *   FILE 312
//*                                                                 *   FILE 312
//*             library will contain a count of dsnames found for   *   FILE 312
//*             the dd followed by the dsnames                      *   FILE 312
//*                                                                 *   FILE 312
//*  Member FINDDSN                                                 *   FILE 312
//*         - added 5/9/19                                          *   FILE 312
//*                                                                 *   FILE 312
//* Function: Find the datasets allocted to a specified ddname      *   FILE 312
//*                                                                 *   FILE 312
//* Usage:    called from a rexx or clist                           *   FILE 312
//*                                                                 *   FILE 312
//*           library = finddsn(ddname)                             *   FILE 312
//*                                                                 *   FILE 312
//*           library will contain a count of dsnames found for     *   FILE 312
//*           the dd followed by the dsnames                        *   FILE 312
//*                                                                 *   FILE 312
//*           For example:                                          *   FILE 312
//*                                                                 *   FILE 312
//*           xx=finddsn(ispmlib);say xx                            *   FILE 312
//*            2 ISP.SISPMENU SYS1.PROD.ISPMENU                     *   FILE 312
//*                                                                 *   FILE 312
//*  Member FIXKEYS - This member is in TSO XMIT format.            *   FILE 312
//*                   Updated 03/18/2024                            *   FILE 312
//*                                                                 *   FILE 312
//*     This is an ISPF command that makes it easy to change PF     *   FILE 312
//*     Key defaults for ALL current ISPF profiles in the users     *   FILE 312
//*     ISPF Profile data set. The current Profile data set         *   FILE 312
//*     is backed up before processing.                             *   FILE 312
//*                                                                 *   FILE 312
//*     - supports changing up to 8 PF Keys at once                 *   FILE 312
//*     - does not affects dialogs with KEYLISTs                    *   FILE 312
//*     - only changes the keys for profiles in the user            *   FILE 312
//*       profile data set and thus may need to be run              *   FILE 312
//*       when new applications (and thus new profiles)             *   FILE 312
//*       are added.                                                *   FILE 312
//*     - when changing the SDSF profile change RETREIVE            *   FILE 312
//*       to CRETRIEV and RFIND to IFIND                            *   FILE 312
//*     - Must update ISPF Config (TSO ISPCCONF) USE_KEYLIST to     *   FILE 312
//*       be able to override some application keys.                *   FILE 312
//*                                                                 *   FILE 312
//*  Member FTPB   - This member is in TSO XMIT format.             *   FILE 312
//*                                                                 *   FILE 312
//*        FTPB - The File Transfer Protocol Batch ISPF Dialog      *   FILE 312
//*             (updated 01/19/2024)                                *   FILE 312
//*                                                                 *   FILE 312
//*     This ISPF dialog provides a simple to use ISPF interface    *   FILE 312
//*     for using the TCP/IP FTP function to transfer data sets     *   FILE 312
//*     from the current MVS host system to other host systems      *   FILE 312
//*     that support a TCP/IP FTP Server (e.g.  MVS, VM, OS/2,      *   FILE 312
//*     most Unix, ...).                                            *   FILE 312
//*                                                                 *   FILE 312
//*     The dialog presents the user with a simple ISPF panel       *   FILE 312
//*     from which to specify the source (original) data set,       *   FILE 312
//*     the target host, optionally the name of the target data     *   FILE 312
//*     set if it is different from the source, and signon          *   FILE 312
//*     information (userid and password).  Once this               *   FILE 312
//*     information is complete the dialog generates the            *   FILE 312
//*     necessary JCL and FTP statements to allow the user to       *   FILE 312
//*     execute the FTP in the foreground (execpt for load          *   FILE 312
//*     library transfers) or to submit the JCL for a batch         *   FILE 312
//*     execution of FTP.  Prior to submission the user is          *   FILE 312
//*     allowed to review and change (edit) the generated JCL       *   FILE 312
//*     and FTP control statements if they desire.                  *   FILE 312
//*                                                                 *   FILE 312
//*  Member GETIPLDT - updated 08/02/2024                           *   FILE 312
//*                                                                 *   FILE 312
//*     A simple exec, using SDSF REXX, to access system info for   *   FILE 312
//*     LPARs within a SYSPLEX and report the IPL Date/Time and     *   FILE 312
//*     z/OS release, etc., for each LPAR.                          *   FILE 312
//*                                                                 *   FILE 312
//*     Note: may also be run under OMVS shell.                     *   FILE 312
//*                                                                 *   FILE 312
//*  Member IEBPDSE - updated 11/01/17 V1.3                         *   FILE 312
//*                                                                 *   FILE 312
//*     A simple ISPF dialog to run IBM's IEBPDSE against your      *   FILE 312
//*     PDSE datasets.                                              *   FILE 312
//*                                                                 *   FILE 312
//*  Member IFTHENEL - ISPF Edit macro                              *   FILE 312
//*                                                                 *   FILE 312
//*     Very simple edit macro to display all if/then/else          *   FILE 312
//*     do/select/when/otherwise/end statements while hiding        *   FILE 312
//*     all others.                                                 *   FILE 312
//*                                                                 *   FILE 312
//*  Member INEWS - This member is in IEBUPDTE SYSIN format.        *   FILE 312
//*                                                                 *   FILE 312
//*     This ISPF application is designed to simplify the task      *   FILE 312
//*     of informing users about system changes, updates,           *   FILE 312
//*     enhancements, etc. each time they logon to TSO and enter    *   FILE 312
//*     ISPF. This is accomplished by a simple modification to      *   FILE 312
//*     the first ISPF menu that the user sees (ISR@PRIM if         *   FILE 312
//*     entry is via command ISPF or ISP@MSTR if entry is via       *   FILE 312
//*     ISPSTART) as documented below.                              *   FILE 312
//*                                                                 *   FILE 312
//*     INEWS is entered by executing the Rexx procedure INEWS      *   FILE 312
//*     and providing one or more of the valid parameters:          *   FILE 312
//*                                                                 *   FILE 312
//*     Syntax:   INEWS parameters                                  *   FILE 312
//*                                                                 *   FILE 312
//*     Required Parameters:                                        *   FILE 312
//*                                                                 *   FILE 312
//*         NEWS      Defines that INEWS will use the NEWS set      *   FILE 312
//*                   of tables, panels, and skeletons.             *   FILE 312
//*         'other'   Must be defined by the installation as        *   FILE 312
//*                   alternative to NEWS.                          *   FILE 312
//*                                                                 *   FILE 312
//*         ***  one of the above is required                       *   FILE 312
//*                                                                 *   FILE 312
//*     Optional Parameters:                                        *   FILE 312
//*         NEW       Display the news ISPF table only if new       *   FILE 312
//*                   or unread items are in the table for the      *   FILE 312
//*                   user                                          *   FILE 312
//*         DEBUG     Used to turn on REXX tracing for              *   FILE 312
//*                   debugging purposes                            *   FILE 312
//*         ADMIN     Enable the administration application         *   FILE 312
//*         TEST      Uses a test news table for testing            *   FILE 312
//*                   purposes.                                     *   FILE 312
//*         FORCE     If the table is locked by ADMIN and the       *   FILE 312
//*                   lock is obsolete (for some reason that        *   FILE 312
//*                   left the member LOCK in the news data         *   FILE 312
//*                   set) this option will override the lock       *   FILE 312
//*                   for administration purposes.                  *   FILE 312
//*                                                                 *   FILE 312
//*     See the rexx procedure for more information.                *   FILE 312
//*                                                                 *   FILE 312
//*     Updates to ISPF Panels ISR@PRIM and/or ISP@MSTR to          *   FILE 312
//*     cause this application to be invoked when the user          *   FILE 312
//*     enters ISPF.                                                *   FILE 312
//*                                                                 *   FILE 312
//*  Member IPLTCHK (added 09/14/2018)                              *   FILE 312
//*                                                                 *   FILE 312
//*        -------------------------------------------------------  *   FILE 312
//*        This REXX helps solve the problem of which DASD volumes  *   FILE 312
//*        connected to your system, contain IPL text, and what     *   FILE 312
//*        IPL text do they contain?                                *   FILE 312
//*        -------------------------------------------------------  *   FILE 312
//*        You don't have to dump Track 0 for ALL of your volumes,  *   FILE 312
//*        but you can FILTER the volser's for strings with volume  *   FILE 312
//*        names that you want to look at.  See syntax below.       *   FILE 312
//*        -------------------------------------------------------  *   FILE 312
//*                                                                 *   FILE 312
//*        Function:  Generate ADRDSSU Step and control cards to    *   FILE 312
//*                   print the first track of the selected disk    *   FILE 312
//*                   volumes.                                      *   FILE 312
//*                                                                 *   FILE 312
//*                   The main purpose is to find the disk          *   FILE 312
//*                   volumes that have IPL Text installed on       *   FILE 312
//*                   them and help to identify which type of IPL   *   FILE 312
//*                   Text using the trusted, real-time,            *   FILE 312
//*                   reliable, always available, and free          *   FILE 312
//*                   utility IEB-EYE-BALL to review.               *   FILE 312
//*                                                                 *   FILE 312
//*        Syntax:    %ipltchk filter(s)                            *   FILE 312
//*                                                                 *   FILE 312
//*                   filters are any strings that must be found    *   FILE 312
//*                   within the volser to be used.                 *   FILE 312
//*                                                                 *   FILE 312
//*        Usage:  Execute with, or without a filter, to generate   *   FILE 312
//*                the ADRDSSU JCL and control statements to        *   FILE 312
//*                print track 0 for the requested volumes. At      *   FILE 312
//*                the end of use the user is placed into ISPF      *   FILE 312
//*                Edit on the results and may then insert a JOB    *   FILE 312
//*                card, tailor however they wish, and submit it.   *   FILE 312
//*                Then review the OUTPUT DD Sysout for the         *   FILE 312
//*                information.                                     *   FILE 312
//*                                                                 *   FILE 312
//*        Dependencies:  DUDASD is required from CBT Tape File 612 *   FILE 312
//*                                                                 *   FILE 312
//*  Member ISPFCMDS                                                *   FILE 312
//*                                                                 *   FILE 312
//*     ISPFCMDS is a utility ISPF command that eases the task      *   FILE 312
//*     of adding installation or user commands to an active        *   FILE 312
//*     ISPF command table. This can eliminaate the requirement     *   FILE 312
//*     to customize the IBM provided ISPF command table or to      *   FILE 312
//*     create elaborate Site or User ISPF command table.           *   FILE 312
//*                                                                 *   FILE 312
//*   Syntax                                                        *   FILE 312
//*                                                                 *   FILE 312
//*     The syntax for calling ISPFCMDS is:                         *   FILE 312
//*                                                                 *   FILE 312
//*        %ISPFCMDS table verb truncation action                   *   FILE 312
//*                                                                 *   FILE 312
//*     Where:                                                      *   FILE 312
//*                                                                 *   FILE 312
//*     table is USER to add the command to the User Command table  *   FILE 312
//*              SITE to add the command to the Site table          *   FILE 312
//*              ISPF to add the command to the ISPCMDS table       *   FILE 312
//*                    note that this option is not recommended     *   FILE 312
//*              * to add the command to one of the following       *   FILE 312
//*                        in this order:                           *   FILE 312
//*                        1) USER                                  *   FILE 312
//*                        2) SITE                                  *   FILE 312
//*                        3) the active Application command table  *   FILE 312
//*                        4) ISPCMDS                               *   FILE 312
//*                                                                 *   FILE 312
//*     verb  is the name of the command to add to the table. This  *   FILE 312
//*                   must be from 1 to 8 alphanumeric characters.  *   FILE 312
//*                                                                 *   FILE 312
//*     truncation is the number of characters which the command    *   FILE 312
//*                   can be abbreviated or 0 to indicate no        *   FILE 312
//*                   abbreviation                                  *   FILE 312
//*                                                                 *   FILE 312
//*     action is a valid ISPF Select command                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member ISPFDEMO  (Added 04/27/2021)                            *   FILE 312
//*                                                                 *   FILE 312
//*    Create a ISPF dialog demo that demonstrates panel flow.      *   FILE 312
//*                                                                 *   FILE 312
//*  Member ISPFLLV   (Added 05/29/2022)                            *   FILE 312
//*                                                                 *   FILE 312
//*    Tool to View both ISPLIST and ISPLOG when those are          *   FILE 312
//*    allocate to SYSOUT. Uses the SDSF REXX API and optionally    *   FILE 312
//*    STEMEDIT (file 895)                                          *   FILE 312
//*                                                                 *   FILE 312
//*  Member LOADISPF  (updated 01/09/2019)                          *   FILE 312
//*                                                                 *   FILE 312
//*    LOADISPF is a rexx routine to be copied into your            *   FILE 312
//*    rexx code that supports placing all ISPF elements            *   FILE 312
//*    (panels, messages, skeletons, clists, and rexx)              *   FILE 312
//*    inline in your REXX exec. It will, when called,              *   FILE 312
//*    scan your source code and dynamically allocate               *   FILE 312
//*    temporary datasets and then altlib or libdef to              *   FILE 312
//*    them.                                                        *   FILE 312
//*                                                                 *   FILE 312
//*  Member LOWER   - Simple REXX function written in REXX to       *   FILE 312
//*                   return a string in lowercase:                 *   FILE 312
//*                                                                 *   FILE 312
//*                   lcase = lower('STRING')                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member LSTPROC - REXX Exec to list PROCLIB libraries and       *   FILE 312
//*                   invoke ISRDDN.                                *   FILE 312
//*                    ** updated 2023/04/14 **                     *   FILE 312
//*                                                                 *   FILE 312
//*  Member LSTPROC3 - version of LSTPROC for JES3 shops            *   FILE 312
//*                    ** updated 9/27/18 **                        *   FILE 312
//*                                                                 *   FILE 312
//*  Member MGEN - simple rexx exec to display the system           *   FILE 312
//*                maxgen limit. Demonstrates how to find           *   FILE 312
//*                the value.                                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member OMVSCMD   ** Updated 01/02/2024                         *   FILE 312
//*                                                                 *   FILE 312
//*              ************************************               *   FILE 312
//*              * Effectively replaced by OMVSCMDS *               *   FILE 312
//*              ************************************               *   FILE 312
//*                                                                 *   FILE 312
//*    Copy the OMVSCMD member from this library into a library     *   FILE 312
//*    in your SYSEXEC, or SYSPROC, allocations and enjoy.          *   FILE 312
//*                                                                 *   FILE 312
//*    Function:  Issue a OMVS command for the passed option        *   FILE 312
//*               or prompt for a command.  Then display the        *   FILE 312
//*               results in ISPF Browse.                           *   FILE 312
//*                                                                 *   FILE 312
//*               If no command is provided then a popup panel      *   FILE 312
//*               appears to prompt for the OMVS command.           *   FILE 312
//*                                                                 *   FILE 312
//*    Syntax:    %OMVSCMD command                                  *   FILE 312
//*               or                                                *   FILE 312
//*               %OMVSCMD -E command  (to Edit the results)        *   FILE 312
//*                                                                 *   FILE 312
//*    Usage:     Best used when added to the site ISPF             *   FILE 312
//*               command table:                                    *   FILE 312
//*                                                                 *   FILE 312
//*               Verb:   ocmd                                      *   FILE 312
//*               T:      0                                         *   FILE 312
//*               Action: select cmd(%OMVSCMD &zparm)               *   FILE 312
//*                                                                 *   FILE 312
//*               Then the user can enter:  ocmd xxx                *   FILE 312
//*                                                                 *   FILE 312
//*    Member OMVSCMDS - Updated 03/28/2025                         *   FILE 312
//*                                                                 *   FILE 312
//*   >>>>>> This is a replacement for OMVSCMD <<<<<<               *   FILE 312
//*                                                                 *   FILE 312
//*    A full ISPF dialog to invoke OMVS shell command with command *   FILE 312
//*    history.                                                     *   FILE 312
//*                                                                 *   FILE 312
//*    Copy the OMVSCMDS member from this library into a library    *   FILE 312
//*    in your SYSEXEC, or SYSPROC, allocations and enjoy.          *   FILE 312
//*                                                                 *   FILE 312
//*    Function:  Issue a OMVS command for the passed option        *   FILE 312
//*               or prompt for a command.  Then display the        *   FILE 312
//*               results in ISPF Browse or View.                   *   FILE 312
//*                                                                 *   FILE 312
//*               If no command is provided then a table of prior   *   FILE 312
//*               commands is displayed which can then be selected. *   FILE 312
//*                                                                 *   FILE 312
//*    Syntax:    %OMVSCMDS command                                 *   FILE 312
//*                                                                 *   FILE 312
//*               command is optional                               *   FILE 312
//*                                                                 *   FILE 312
//*    Usage:     Best used when added to the site ISPF             *   FILE 312
//*               command table:                                    *   FILE 312
//*                                                                 *   FILE 312
//*               Verb:   ocmd                                      *   FILE 312
//*               T:      0                                         *   FILE 312
//*               Action: select cmd(%OMVSCMDS &zparm)              *   FILE 312
//*                                                                 *   FILE 312
//*               Then the user can enter:  ocmd xxx                *   FILE 312
//*                                                                 *   FILE 312
//*    Member OMVSCOPY - Updated 08/10/2018                         *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSCOPY contains the following members:                     *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSCOPY  - The ISPF front-end to the TSO OCOPY Command      *   FILE 312
//*    OCOPYO    - Sample JCL: copy from OMVS file to z/OS data set *   FILE 312
//*    OCOPYZ    - Sample JCL: copy from z/OS data set to OMVS file *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSCOPY is an ISPF front-end to the TSO OCOPY command       *   FILE 312
//*    designed to make it easy to copy an z/OS data set to an OMVS *   FILE 312
//*    file and vice versa.  OMVSCOPY supports both foreground and  *   FILE 312
//*    batch execution. When the Batch option is selected, it will  *   FILE 312
//*    dynamically generate the batch JCL and allow the user to     *   FILE 312
//*    Edit it prior to submission, or the user can copy the JCL to *   FILE 312
//*    a permanent JCL data set for modification and reuse.         *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSCOPY is an ISPF front end to the IBM TSO OCOPY command   *   FILE 312
//*    and will:                                                    *   FILE 312
//*                                                                 *   FILE 312
//*    1. copy a z/OS data set to an OMVS file                      *   FILE 312
//*    2. copy an OMVS file to a z/OS data set                      *   FILE 312
//*    3. supports an ISPF 3.17 like interface to find and select   *   FILE 312
//*       the desired OMVS file to copy                             *   FILE 312
//*    4. supports a ISPF 3.4 like interface to find and select the *   FILE 312
//*       desired z/OS data set to copy                             *   FILE 312
//*    5. supports a member selection list interface to find and    *   FILE 312
//*       select the desired PDS member to copy                     *   FILE 312
//*    6. Foreground and Batch execution is supported with the      *   FILE 312
//*       Batch mode generating JCL, presented under ISPF Edit, to  *   FILE 312
//*       the user to submit or to copy for later use.              *   FILE 312
//*    7. Support for SuperUser (foreground only)                   *   FILE 312
//*                                                                 *   FILE 312
//*    While using the ISPF dialog the input supports               *   FILE 312
//*    special processing:                                          *   FILE 312
//*                                                                 *   FILE 312
//*       - hlq.xxx.*    Results in a selection list of available   *   FILE 312
//*                      data sets                                  *   FILE 312
//*       - hlq.xxx.pds  Results in a selection list of members     *   FILE 312
//*       - /u/          Results in a selection list of OMVS files  *   FILE 312
//*                      similar to ISPF 3.17                       *   FILE 312
//*                                                                 *   FILE 312
//*    When in the OMVS file selection display the user can use L   *   FILE 312
//*    to open a directory, including using L on the .. directory   *   FILE 312
//*    to move up one level.  The CD command may also be used to go *   FILE 312
//*    directy to a directory. And the ~ may be used to indicate    *   FILE 312
//*    the users home directory.                                    *   FILE 312
//*                                                                 *   FILE 312
//*    The sample JCL members are for those who prefer to do the    *   FILE 312
//*    copy in batch.                                               *   FILE 312
//*                                                                 *   FILE 312
//*    Member OMVSMAN - updated 02/27/25                            *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSMAN is an ISPF dialog that will list all of the known    *   FILE 312
//*    OMVS man pages in an ISPF Table. The manpage and description *   FILE 312
//*    is displayed. The user can select a manpage to be displayed  *   FILE 312
//*    in ISPF Browse or View.                                      *   FILE 312
//*                                                                 *   FILE 312
//*    Includes support for the zopen tools man pages               *   FILE 312
//*                                                                 *   FILE 312
//*    The REXX code contains the ISPF Panels and Message inline    *   FILE 312
//*    so this is easy to install and use.                          *   FILE 312
//*                                                                 *   FILE 312
//*    Member OMVSPAX - this member is in TSO XMIT format.          *   FILE 312
//*               ** Updated 09/17/2020                             *   FILE 312
//*                                                                 *   FILE 312
//*    This member, when received using TSO RECEIVE, will be a      *   FILE 312
//*    PDS with the package.  Member $DOC is additional             *   FILE 312
//*    documentation, Member $RECV will receive the EXEC and        *   FILE 312
//*    PANELS members to create an EXEC and PANELS library.         *   FILE 312
//*                                                                 *   FILE 312
//*    OMVSPAX is a package of three small ISPF dialogs             *   FILE 312
//*    written in REXX to simplify the backup and restoration       *   FILE 312
//*    of a omvs directory.                                         *   FILE 312
//*     The dialogs are:                                            *   FILE 312
//*                                                                 *   FILE 312
//*         OMVSPAXB  - backup a omvs directory using pax to a      *   FILE 312
//*                     z/OS dataset.                               *   FILE 312
//*         OMVSPAXL  - list the contents of a backup pax z/OS      *   FILE 312
//*                     dataset.                                    *   FILE 312
//*         OMVSPAXR  - restore a pax z/OS backup dataset to        *   FILE 312
//*                     the original omvs directory or another      *   FILE 312
//*                     directory providing it exists               *   FILE 312
//*                                                                 *   FILE 312
//*     To invoke the dialogs:                                      *   FILE 312
//*                                                                 *   FILE 312
//*         1. Must be under ISPF                                   *   FILE 312
//*         2. From ISPF 6 enter %OMVSPAX?   Where ? is B/L/R       *   FILE 312
//*         3. From any ISPF command line enter:  TSO %OMVSPAX?     *   FILE 312
//*                                                                 *   FILE 312
//*  Member OMVSSEL - ISPF REXX Subroutine to Select OMVS Files     *   FILE 312
//*               ** Updated 08/16/2018                             *   FILE 312
//*                                                                 *   FILE 312
//*     Very useful subroutine for use in REXX under ISPF to        *   FILE 312
//*     select an OMVS file from a ISPF 3.17 like display for       *   FILE 312
//*     processing.                                                 *   FILE 312
//*                                                                 *   FILE 312
//*  Member OMVSTRY - TSO interface to OMVS/Shell commands          *   FILE 312
//*               ** Addfed 03/27/2025                              *   FILE 312
//*                                                                 *   FILE 312
//*     Similar to REXXTRY but for OMVS/Shell commands              *   FILE 312
//*                                                                 *   FILE 312
//*  Member ONCALL - Generate an oncall rotation schedule           *   FILE 312
//*                                                                 *   FILE 312
//*    I have a new tool that is on my beta page that you           *   FILE 312
//*    all might find interesting.  It will generate an             *   FILE 312
//*    oncall rotation for your group and optionally e-mail         *   FILE 312
//*    (using xmitip) the rotation list along with an               *   FILE 312
//*    icalendar file that can be used to add the oncall            *   FILE 312
//*    information to each individuals calendar.                    *   FILE 312
//*                                                                 *   FILE 312
//*  Member ONLY                                                    *   FILE 312
//*               ** Updated 12/24/2019                             *   FILE 312
//*                                                                 *   FILE 312
//*    ISPF Edit ONLY command to hide all records and expose only   *   FILE 312
//*    those that match the provided criteria.                      *   FILE 312
//*                                                                 *   FILE 312
//*  Member PDS2PDSE  - TSO command (REXX) to convert a PDS         *   FILE 312
//*                     to a PDSE with member generations           *   FILE 312
//*               ** Updated 2020-05-31                             *   FILE 312
//*                                                                 *   FILE 312
//*     Syntax: pds2pdse from-pds to-pdse mg(nnn) vol(vvv) swap     *   FILE 312
//*                                                                 *   FILE 312
//*     mg is the maxgen limit - defaults to system limit           *   FILE 312
//*     swap will rename the datasets after the alloc/copy          *   FILE 312
//*                                                                 *   FILE 312
//*     * Requires the PDS command (file 182)                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member PLPISPF - A Dynamic ISPF Menu System                    *   FILE 312
//*               ** Updated 10/16/2018                             *   FILE 312
//*                                                                 *   FILE 312
//*     PLPISPF, or PLP for short, is a dynamic ISPF menuing        *   FILE 312
//*     system. PLP is short for Product Launch Point. It has       *   FILE 312
//*     a full ISPF menu driven administrative component that       *   FILE 312
//*     allows the admin to define the application name, profile,   *   FILE 312
//*     load library, clist/exec library, other ispf libraries,     *   FILE 312
//*     and optionally additional DD's to allocate. Then the        *   FILE 312
//*     call using TSO command, ISPF command, or ISPF Panel.        *   FILE 312
//*                                                                 *   FILE 312
//*  Member PNS - a short text document                             *   FILE 312
//*                                                                 *   FILE 312
//*     Attempts to document how to use point and shoot fields      *   FILE 312
//*     in ISPF dialogs.                                            *   FILE 312
 /*                                                                 *   FILE 312
//*  Member PRINT - This member is in TSO XMIT format.              *   FILE 312
//*               ** Updated 2/14/18 **                             *   FILE 312
//*                                                                 *   FILE 312
//*     This member contains 2 ISPF dialogs:                        *   FILE 312
//*                                                                 *   FILE 312
//*     LPREDIT  - ISPF Edit command to invoke LPRPRINT             *   FILE 312
//*                                                                 *   FILE 312
//*     LPRPRINT - used to print using the z/OS TCP/IP LPR          *   FILE 312
//*                command to any system with an LPD server.        *   FILE 312
//*                This includes intelligent printers which         *   FILE 312
//*                have LPD build-in. Now with message and panels   *   FILE 312
//*                inline.                                          *   FILE 312
//*                                                                 *   FILE 312
//*     PSPRINT  - used to format host output for printing on a     *   FILE 312
//*                PostScript printer and then invoke LPRPRINT.     *   FILE 312
//*                Options include Portrait, Landscape, and 2UP     *   FILE 312
//*                printing.                                        *   FILE 312
//*                                                                 *   FILE 312
//*     The members of this dataset are in IEBUPDTE format.         *   FILE 312
//*                                                                 *   FILE 312
//*     $DOC     - What you are reading                             *   FILE 312
//*     EXEC     - The above 3 rexx execs which are the entry       *   FILE 312
//*                points to the dialogs                            *   FILE 312
//*     MSGS     - ISPF messages for PSPRINT                        *   FILE 312
//*     PANELS   - ISPF panels, including brief tutorials, for      *   FILE 312
//*                the PSPRINT dialog                               *   FILE 312
//*                                                                 *   FILE 312
//*  Member PRMCK - Check the syntax of PARMLIB members.            *   FILE 312
//*         Updated 10/01/21                                        *   FILE 312
//*                                                                 *   FILE 312
//*     PARMLIB Check                                               *   FILE 312
//*                                                                 *   FILE 312
//*     This application consists of a REXX Exec and an ISPF        *   FILE 312
//*     Panel.  To use this you need to copy the exec (choose       *   FILE 312
//*     the FB or the VB version) into a library in your            *   FILE 312
//*     SYSPROC or SYSEXEC concatenation.  You then need to         *   FILE 312
//*     copy the panel into a library in your ISPPLIB               *   FILE 312
//*     concatenation.                                              *   FILE 312
//*                                                                 *   FILE 312
//*     Usage is to Edit the desired member of SYS1.PARMLIB         *   FILE 312
//*     and enter the command PRMCK.                                *   FILE 312
//*                                                                 *   FILE 312
//*     Syntax: PRMCK cat sysres (debug                             *   FILE 312
//*                                                                 *   FILE 312
//*     valid options are:                                          *   FILE 312
//*           ?   - will prompt for catalog and sysres              *   FILE 312
//*           -H  - display tutorial panel                          *   FILE 312
//*           cat - is a name that will be used in the master       *   FILE 312
//*                 catalog lookup (find *custom* below) and        *   FILE 312
//*                 if not found will be used as the master         *   FILE 312
//*                 catalog name (enter without quotes).            *   FILE 312
//*           sysres is the volser of the system ipl volume         *   FILE 312
//*                 to be checked when a volser of ****** is        *   FILE 312
//*                 coded.                                          *   FILE 312
//*           (debug - will turn on tracing                         *   FILE 312
//*                                                                 *   FILE 312
//*     Support for PROGxx member statements                        *   FILE 312
//*        - LNKLST                                                 *   FILE 312
//*        - APF                                                    *   FILE 312
//*        - LPA                                                    *   FILE 312
//*        - SYSLIB                                                 *   FILE 312
//*     Support for LNKLSTxx and LPALSTxx members                   *   FILE 312
//*                                                                 *   FILE 312
//*     Verification is not 100% the same as the system will        *   FILE 312
//*     perform when used but it does a fair amount of              *   FILE 312
//*     verification.  Errors and Warnings are inserted into        *   FILE 312
//*     the Edit display as non-saveable messages.                  *   FILE 312
//*                                                                 *   FILE 312
//*     Member QTAB     - Updated 23/04/03                          *   FILE 312
//*                                                                 *   FILE 312
//*     Function:  ISPF Dialog to display all open ISPF tables      *   FILE 312
//*                with table stats with an option to display       *   FILE 312
//*                all table rows. Very useful to debug an ISPF     *   FILE 312
//*                application to see if it leaves any open         *   FILE 312
//*                tables when it ends.                             *   FILE 312
//*                                                                 *   FILE 312
//*                Updated to support row extension variables.      *   FILE 312
//*                                                                 *   FILE 312
//*     Member RANDSTR  - Updated 02/27/2018                        *   FILE 312
//*                                                                 *   FILE 312
//*     Function:  Generate a unique character string for use       *   FILE 312
//*                in an ISPF Table name, DDName, etc.              *   FILE 312
//*                                                                 *   FILE 312
//*                This is for ISPF dialogs that may run            *   FILE 312
//*                concurrently in either multiple split            *   FILE 312
//*                screens or stacked so as to prevent duplicate    *   FILE 312
//*                DD or ISPF table names.                          *   FILE 312
//*                                                                 *   FILE 312
//*                Or any length string with or without             *   FILE 312
//*                lowercase characters.                            *   FILE 312
//*                                                                 *   FILE 312
//*                Thus this can be used to generate a random       *   FILE 312
//*                password or passphrase                           *   FILE 312
//*                                                                 *   FILE 312
//*                This may also be used for any other need         *   FILE 312
//*                to have a unique character string that is        *   FILE 312
//*                a valid DDName, Member Name, etc.                *   FILE 312
//*                                                                 *   FILE 312
//*     Syntax:    x = randstr(n)                                   *   FILE 312
//*                                                                 *   FILE 312
//*                Where n is the number of characters to           *   FILE 312
//*                return, always starting with an alpha.           *   FILE 312
//*                                                                 *   FILE 312
//*                The default if not provided is 8                 *   FILE 312
//*                                                                 *   FILE 312
//*                If 'n' is preceded by L (e.g. L8) then           *   FILE 312
//*                50% of the characters will be lowercase          *   FILE 312
//*                                                                 *   FILE 312
//*  Member RELPDSE                                                 *   FILE 312
//*         - updated 01/04/2023                                    *   FILE 312
//*                                                                 *   FILE 312
//*    Invoke ADRDSSU to do a partial release of space in a PDSE.   *   FILE 312
//*    Thanks to code provided by Pedro Vera.                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member REXXER                                                  *   FILE 312
//*         - added 10/28/20                                        *   FILE 312
//*                                                                 *   FILE 312
//*    Invoke REXX Compiler and only display error messages as      *   FILE 312
//*    an ISPF Edit Macro.                                          *   FILE 312
//*                                                                 *   FILE 312
//*  Member REXXFORM                                                *   FILE 312
//*                                                                 *   FILE 312
//*    REXXFORM is the z/OS ISPF Edit macro ported from the         *   FILE 312
//*    popular z/VM XEDIT REXXFORM command with several minor       *   FILE 312
//*    enhancements to take advantage of ISPF Edit capabilities.    *   FILE 312
//*                                                                 *   FILE 312
//*    REXXFORM is an ISPF edit macro used to format REXX           *   FILE 312
//*    EXECs by indenting DO and SELECT groups and                  *   FILE 312
//*    left-justifying lines at a selected column.  It also         *   FILE 312
//*    checks for unbalanced DO or SELECT statements.  One          *   FILE 312
//*    use of this ISPF edit macro is to uniformly                  *   FILE 312
//*    restructure REXX files after composing them without          *   FILE 312
//*    regard for any particular format or standard coding          *   FILE 312
//*    style.                                                       *   FILE 312
//*                                                                 *   FILE 312
//*  Member REXXTRY                                                 *   FILE 312
//*                                                                 *   FILE 312
//*    REXXTRY is from IBM's OS/2 and is an interactive             *   FILE 312
//*    way to experiment with any REXX command you care             *   FILE 312
//*    to try.                                                      *   FILE 312
//*                                                                 *   FILE 312
//*                                                                 *   FILE 312
//*  Member RUNC    - this member is in TSO XMIT format.            *   FILE 312
//*                   Updated 07/30/2020                            *   FILE 312
//*                                                                 *   FILE 312
//*    The RUNC ISPF Edit Command is only used within ISPF Edit     *   FILE 312
//*    and will execute any TSO commands found on the selected      *   FILE 312
//*    records within the active ISPF Edit data.                    *   FILE 312
//*                                                                 *   FILE 312
//*    No knowledge of CLIST, REXX, or JCL is required to use.      *   FILE 312
//*    But knowing TSO commands is helpful :-)                      *   FILE 312
//*                                                                 *   FILE 312
//*    NEW Capability to execute an Inline ISPF Edit Macro.         *   FILE 312
//*                                                                 *   FILE 312
//*    Syntax:  RUNC options                                        *   FILE 312
//*                                                                 *   FILE 312
//*    options may be:                                              *   FILE 312
//*                                                                 *   FILE 312
//*               blank (default)                                   *   FILE 312
//*               ? or HELP to display this info                    *   FILE 312
//*               n - must be the first option and will skip        *   FILE 312
//*                   the first n characters to find the command    *   FILE 312
//*               ? or HELP to display help information             *   FILE 312
//*              -A process all non-excluded command records        *   FILE 312
//*              -ALL process all non-excluded command records      *   FILE 312
//*              -B to browse the results using STEMEDIT            *   FILE 312
//*              -C to display log datasets                         *   FILE 312
//*              -D to insert messages as data in edit session      *   FILE 312
//*                 or -D(prefix) to prefix the inserted messages   *   FILE 312
//*              -L to log to a dataset (default defined in code)   *   FILE 312
//*              -LD to log to a sequential dataset                 *   FILE 312
//*              -LP to log to a partitioned dataset                *   FILE 312
//*              -LX to over-ride logging if defaulted in userdefs  *   FILE 312
//*              -N to insert messages as notelines in edit session *   FILE 312
//*              -O to change user default RUNC options             *   FILE 312
//*              -R to generate report if no messages generated     *   FILE 312
//*              -S nnn to stop if the return code exceeds nnn      *   FILE 312
//*              -T to not trap and let the results go to screen    *   FILE 312
//*              -V to view the results using STEMEDIT              *   FILE 312
//*                  default is to View                             *   FILE 312
//*              -W nnn to wrap text for -D/-N to nnn characters    *   FILE 312
//*                 if nnn is W will wrap to Edit data length       *   FILE 312
//*              ONLY(string) will search for the string (e.g. xyz) *   FILE 312
//*                 in the command string and if not found will     *   FILE 312
//*                 ignore that command.                            *   FILE 312
//*              PREFIX(string) will append the string to the       *   FILE 312
//*                 front of each command.                          *   FILE 312
//*              SUFFIX(string) will append the string to the       *   FILE 312
//*                 end of each command.                            *   FILE 312
//*                                                                 *   FILE 312
//*              ** PREFIX and SUFFIX apply only for TSO commands   *   FILE 312
//*                                                                 *   FILE 312
//*   Special control statements:                                   *   FILE 312
//*              <DOC><TITLE></DOC> for a doc pop up panel          *   FILE 312
//*              <EXIT rc> to exit if return code >=                *   FILE 312
//*              <START><END> to define a range of commands         *   FILE 312
//*                                                                 *   FILE 312
//*              SET symbolic = value                               *   FILE 312
//*                                                                 *   FILE 312
//*    Dependencies: Requires STEMEDIT (copy included in package)   *   FILE 312
//*                  Optional EKKO (copy included in package)       *   FILE 312
//*                                                                 *   FILE 312
//*    Usage Notes: 1. Select records with TSO commands using       *   FILE 312
//*                    line tags, C, C#, or CC and CC,              *   FILE 312
//*                    or S, S#, SS and SS.                         *   FILE 312
//*                 2. Use the command option of -ALL to process    *   FILE 312
//*                    all non-excluded records for commands        *   FILE 312
//*                 3. Data lines starting with *, /*, //, or //*   *   FILE 312
//*                    or all blank will be ignored                 *   FILE 312
//*                    - use n to skip over *, /* , //, or //*      *   FILE 312
//*                 4. Excluded lines are also ignored              *   FILE 312
//*                 5. Commands may be continued on the next        *   FILE 312
//*                    record by using a + at the end of the        *   FILE 312
//*                    command for the record                       *   FILE 312
//*                 6. The data on the line will be executed        *   FILE 312
//*                    using the Address TSO command as a TSO       *   FILE 312
//*                    command, or ADDRESS ISPExec for ISPF         *   FILE 312
//*                    commands.                                    *   FILE 312
//*                 7. TSO and ISPF SELECT commands can be in any   *   FILE 312
//*                    record in the data.                          *   FILE 312
//*                 8. Not all TSO commands are trappable           *   FILE 312
//*                    - only those that use PUTLINE                *   FILE 312
//*                    - ISPF commands probably are not             *   FILE 312
//*                 9. Symbolics are supported in the command       *   FILE 312
//*                    using the syntax of &symbol. An ISPF         *   FILE 312
//*                    panel will be generated to prompt for        *   FILE 312
//*                    the symbolic values.                         *   FILE 312
//*                10. Use a symbolic at the end to allow entry     *   FILE 312
//*                    of additional command options                *   FILE 312
//*                11. Over 20 predefined symbolics supported       *   FILE 312
//*                                                                 *   FILE 312
//*     Sample Usage:                                               *   FILE 312
//*                                                                 *   FILE 312
//*        LISTD &dsn                                               *   FILE 312
//*        LISTC ENT(&dsn) ALL                                      *   FILE 312
//*        PDS &dsn                                                 *   FILE 312
//*        PDS MY.EXEC                                              *   FILE 312
//*        SELECT PANEL(&panel)                                     *   FILE 312
//*        SELECT PANEL(ISR@PRIM) +                                 *   FILE 312
//*               opt(&opt)                                         *   FILE 312
//*        BROWSE Dataset(xxx)                                      *   FILE 312
//*        BROWSE Dataset(xxx) Volume(volser)                       *   FILE 312
//*        BROWSE Member(xxx)                                       *   FILE 312
//*        Edit Dataset(xxx)                                        *   FILE 312
//*        Edit Dataset(xxx) Volume(volser)                         *   FILE 312
//*        Edit Member(xxx)                                         *   FILE 312
//*        View Dataset(xxx)                                        *   FILE 312
//*        View Dataset(xxx) Volume(volser)                         *   FILE 312
//*        View Member(xxx)                                         *   FILE 312
//*        Rename dataset volser from-member to-member              *   FILE 312
//*        Sleep nn                                                 *   FILE 312
//*        EJES ST                                                  *   FILE 312
//*        SDSF ST                                                  *   FILE 312
//*                                                                 *   FILE 312
//*    Then use the RUNC command on that dataset/member and use the *   FILE 312
//*    row selection commands to select the record(s) to process.   *   FILE 312
//*                                                                 *   FILE 312
//*    Included is the ERC (execute runc) command that is a ispf    *   FILE 312
//*    command to fast path to the commands dataset or pds member.  *   FILE 312
//*                                                                 *   FILE 312
//*    The symbolics in the sample commands will bring up an ISPF   *   FILE 312
//*    panel that will prompt the user to enter a value for each    *   FILE 312
//*    symbolic in the order that they are found within the         *   FILE 312
//*    command.                                                     *   FILE 312
//*                                                                 *   FILE 312
//* --------------------------------------------------------------- *   FILE 312
//*     Lionel B. Dyck                                              *   FILE 312
//*     email:   lbdyck@gmail.com                                   *   FILE 312
//*     github:  github.com/lbdyck                                  *   FILE 312
//* --------------------------------------------------------------- *   FILE 312
//*                                                                 *   FILE 312
```
