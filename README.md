# JCL-Run-ReadandWritewithIF

//LIT0047  JOB  UNIVER,CLASS=A,MSGCLASS=H,NOTIFY=&SYSUID                00010079
//JOBLIB   DD   DSN=LIT0047.LYIT11.LOADLIB,DISP=SHR                     00014078
//RUNIT    EXEC PGM=C0161115                                            00015087
//SYSPRINT DD   SYSOUT=*                                                00018075
//ITRANS   DD   DSN=LIT0047.LYIT11.DATA.ITRANS.C0910181,DISP=SHR        00018181
//*OREPORT DD SYSOUT=*,DCB=(RECFM=FBA,LRECL=80,BLKSIZE=0)               00020082
//OREPORT  DD DSN=LIT0047.LYIT11.DATA.OREPORT.C0910183,                 00030087
//            DISP=(NEW,CATLG,DELETE),                                  00040087
//            SPACE=(TRK,(1,1),RLSE),                                   00050087
//            DCB=(RECFM=FBA,LRECL=101,BLKSIZE=0)                       00060087
//*                                                                     00061085
//OMRTRANS DD DSN=LIT0047.LYIT11.DATA.OMRTRANS,                         00070085
//            DISP=(NEW,CATLG,DELETE),                                  00080085
//            SPACE=(TRK,(1,1),RLSE),                                   00090085
//            DCB=(RECFM=FBA,LRECL=70,BLKSIZE=0)                        00100087
 
