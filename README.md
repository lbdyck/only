# Only ISPF Edit Macro

ONLY is an ISPF Edit command that will find all occurrences of a string          
and hide all records that do not include that string. An optional second         
string will further limit the display of records that include both strings       
                                                                                 
Syntax:  ONLY string-1 string-2 find-options                                     
      or ONLY ?                                                                  
                                                                                 
         ? will display this ISPF Tutorial                                       
         string-1 and string-2 must be enclosed in quotes if blanks included     
         * may only be in string-2                                               
         use of an & will make both string case sensitive                        
         find-options are any find options (e.g. word prefix label column) *     
             * these only apply to string-1                                      
                                                                                 
Examples:                                                                        
                                                                                 
         ONLY EXEC PGM                                                           
         - will display only JCL statements that exec a program and not proc     
