# CBT996
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)
This is still a work in progress. GitHub repos will be deleted and created during this period...
~~~~~~~~~~~~~~~~

//***FILE 996 is from Larry K. Slaten and contains several packages *   FILE 996
//*           of useful programs.                                   *   FILE 996
//*                                                                 *   FILE 996
//*           email:  larry.k.slaten@gmail.com                      *   FILE 996
//*                                                                 *   FILE 996
//*    The following members contain user documents (in MS Word     *   FILE 996
//*    format) for the load library scanner, the REXX Toolkit,      *   FILE 996
//*    and the String handling package.                             *   FILE 996
//*                                                                 *   FILE 996
//*    @LIBSCAN - Document describing the load library scanner      *   FILE 996
//*    @REXTOOL - Document describing the REXX Toolkit              *   FILE 996
//*    @STRING  - Document describing the String Handling Package   *   FILE 996
//*                                                                 *   FILE 996
//*    (These members must be downloaded to a PC in BINARY and      *   FILE 996
//*    looked at with a PDF reader such as Adobe.)                  *   FILE 996
//*                                                                 *   FILE 996
//*    The IEBUPDT1 member is setup to install all source           *   FILE 996
//*    libraries.                                                   *   FILE 996
//*    * &TGTHLQ.ASUTIL.ASM      assembler source                   *   FILE 996
//*    * &TGTHLQ.ASUTIL.CNTL     JCL source                         *   FILE 996
//*    * &TGTHLQ.ASUTIL.COBOL    COBOL source                       *   FILE 996
//*    * &TGTHLQ.BATCH.REXXJCL   JCL to run batch REXX              *   FILE 996
//*    * &TGTHLQ.BATCH.REXXLIB   batch REXX source                  *   FILE 996
//*    * &TGTHLQ.MYTSO.EXEC      REXX Toolkit source                *   FILE 996
//*    * &TGTHLQ.WORK.MODEL      IDCAMS CTL STMT models             *   FILE 996
//*                                                                 *   FILE 996
//*    Compile and Installation Verification Process (IVP)          *   FILE 996
//*    instructions can be found in member $DIR of library          *   FILE 996
//*    &TGTHLQ.ASUTIL.CNTL.                                         *   FILE 996
//*                                                                 *   FILE 996
//*    Member(s) $$UPDTnn contain release changes.                  *   FILE 996
//*                                                                 *   FILE 996
//*    All programs (HLASM and COBOL) are LE conforming.            *   FILE 996
//*                                                                 *   FILE 996
//*    The load library scanner (SSLEANAL) can be used to           *   FILE 996
//*    inventory load libraries (all or selected members).          *   FILE 996
//*    Program dynamically loads members in region storage and      *   FILE 996
//*    collects and prints information.  Check @LIBSCAN document    *   FILE 996
//*    for details.                                                 *   FILE 996
//*                                                                 *   FILE 996
//*    Query Program Object Information (ASU3QOIB) callable         *   FILE 996
//*    program that dynamically loads selected members in region    *   FILE 996
//*    storage and collects information that is returned via        *   FILE 996
//*    a communication area (optional print).                      *   FFILE 996
//*                                                                 *   FILE 996
//*    Binder utility (ASU3BNDB) to print information about an      *   FILE 996
//*    an executable by interfacing with the IBM Binder API for     *   FILE 996
//*    selected members and CSECT(s).                               *   FILE 996
//*    Six different reports can be selected via PARM statement.    *   FILE 996
//*    * History information (IRDx and CUI)                         *   FILE 996
//*    * Map information (similar to a link map)                    *   FILE 996
//*    * Binder Option(s)information                                *   FILE 996
//*    * Module information (similar to COBANAL CBT FILE#321)       *   FILE 996
//*    * ESD information                                            *   FILE 996
//*    * DUMP first 32K of binder buffer                            *   FILE 996
//*                                                                 *   FILE 996
//*    Query Environment Information (ASU3QEIB) callable program    *   FILE 996
//*    that collects information from many of the MVS control       *   FILE 996
//*    blocks that is returned via a communication area (optional   *   FILE 996
//*    print).  This program may require modification for each      *   FILE 996
//*    and every z/OS release.                                      *   FILE 996
//*                                                                 *   FILE 996
//*    The Rexx Toolkit contains many TSO/ISPF/ISREDIT macros.      *   FILE 996
//*    Check @REXTOOL document for details.                         *   FILE 996
//*                                                                 *   FILE 996
//*    Using the Rexx String Functions as a model, I created an     *   FILE 996
//*    assembler subroutine package, providing similar services.    *   FILE 996
//*    The String subroutines can be installed as individual        *   FILE 996
//*    services and/or combined in one executable.                  *   FILE 996
//*    * append source string to result string                      *   FILE 996
//*    * find string, forward scan Boyer-Moore method               *   FILE 996
//*    * return source string centered in result string             *   FILE 996
//*    * return source string de-edited in result string            *   FILE 996
//*    * find string, forward scan TRT method                       *   FILE 996
//*    * return source string as two result strings (chr,hex)       *   FILE 996
//*    * return source string left justified in result string       *   FILE 996
//*    * find string, backward scan TRTR method                     *   FILE 996
//*    * return source string right justified in result string      *   FILE 996
//*    * return source string character and word count in result    *   FILE 996
//*    * return source string with inserted string in result        *   FILE 996
//*    * return source sub-string in result string                  *   FILE 996
//*    * return source string stripped of leading and/or trailing   *   FILE 996
//*      strip characters in result string                          *   FILE 996
//*    * return source string as three result strings (chr,zone,nbr)*   FILE 996
//*    * return source string justified in result string            *   FILE 996
//*    * return source string spaced in result string               *   FILE 996
//*    * return source string less deleted word in result string    *   FILE 996
//*    * return position and text of nth word in source string      *   FILE 996
//*    * return source string less sub-string in result string      *   FILE 996
//*    * return source string with replacing sub-string in result   *   FILE 996
//*    * return lexemes from source string via patterns             *   FILE 996
//*    Check @STRING document for details,                          *   FILE 996
//*                                                                 *   FILE 996
//*    A number of other assembler macros, assembler and COBOL      *   FILE 996
//*    sub-programs, programs, and copybooks are included.          *   FILE 996
//*    * numeric test                                               *   FILE 996
//*    * register 14 stack                                          *   FILE 996
//*    * vector dope vector(s)                                      *   FILE 996
//*    * data wrangling                                             *   FILE 996
//*    * binary search (4 macro variations)                         *   FILE 996
//*    * fibonaccian search                                         *   FILE 996
//*    * linear search                                              *   FILE 996
//*    * heap sort                                                  *   FILE 996
//*    * Dr. John EhrmanÆs bit handling ôMicro-Compilerö.           *   FILE 996
//*    * date processing                                            *   FILE 996
//*    * record length, block length, CISZ, analysis                *   FILE 996
//*                                                                 *   FILE 996
//*    &TGTHLQ.WORK.MODEL contains the IDCAMS control card models   *   FILE 996
//*    for the batch Rexx macro (BLDIDC) in &TGTHLQ.BATCH.REXXLIB   *   FILE 996
//*    library.                                                     *   FILE 996
//*                                                                 *   FILE 996
~~~~~~~~~~~~~~~~

