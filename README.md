 <!-- ======================== Introduction ============================== -->
  <!-- This document defines default values for *all* web applications      -->
  <!-- loaded into this instance of Tomcat.  As each application is         -->
  <!-- deployed, this file is processed, followed by the                    -->
  <!-- "/WEB-INF/web.xml" deployment descriptor from your own               -->
  <!-- applications.                                                        -->
  <!--                                                                      -->
  <!-- WARNING:  Do not configure application-specific resources here!      -->
  <!-- They should go in the "/WEB-INF/web.xml" file in your application.   -->


  <!-- ================== Built In Servlet Definitions ==================== -->


  <!-- The default servlet for all web applications, that serves static     -->
  <!-- resources.  It processes all requests that are not mapped to other   -->
  <!-- servlets with servlet mappings (defined either here or in your own   -->
  <!-- web.xml file).  This servlet supports the following initialization   -->
  <!-- parameters (default values are in square brackets):                  -->
  <!--                                                                      -->
  <!--   debug               Debugging detail level for messages logged     -->
  <!--                       by this servlet. Useful values are 0, 1, and   -->
  <!--                       11 where higher values mean more detail. [0]   -->
  <!--                                                                      -->
  <!--   fileEncoding        Encoding to be used to read static resources   -->
  <!--                       [platform default]                             -->
  <!--                                                                      -->
  <!--   useBomIfPresent     If a static file contains a byte order mark    -->
  <!--                       (BOM), should this be used to determine the    -->
  <!--                       file encoding in preference to fileEncoding.   -->
  <!--                       [true]                                         -->
  <!--                                                                      -->
  <!--   input               Input buffer size (in bytes) when reading      -->
  <!--                       resources to be served.  [2048]                -->
  <!--                                                                      -->
  <!--   listings            Should directory listings be produced if there -->
  <!--                       is no welcome file in this directory?  [false] -->
  <!--                       WARNING: Listings for directories with many    -->
  <!--                       entries can be slow and may consume            -->
  <!--                       significant proportions of server resources.   -->
  <!--                                                                      -->
  <!--   output              Output buffer size (in bytes) when writing     -->
  <!--                       resources to be served.  [2048]                -->
  <!--                                                                      -->
  <!--   readonly            Is this context "read only", so HTTP           -->
  <!--                       commands like PUT and DELETE are               -->
  <!--                       rejected?  [true]                              -->
  <!--                                                                      -->
  <!--   readmeFile          File to display together with the directory    -->
  <!--                       contents. [null]                               -->
  <!--                                                                      -->
  <!--   sendfileSize        If the connector used supports sendfile, this  -->
  <!--                       represents the minimal file size in KB for     -->
  <!--                       which sendfile will be used. Use a negative    -->
  <!--                       value to always disable sendfile.  [48]        -->
  <!--                                                                      -->
  <!--   useAcceptRanges     Should the Accept-Ranges header be included    -->
  <!--                       in responses where appropriate? [true]         -->
  <!--                                                                      -->
  <!--  For directory listing customization. Checks localXsltFile, then     -->
  <!--  globalXsltFile, then defaults to original behavior.                 -->
  <!--                                                                      -->
  <!--   localXsltFile       Make directory listings an XML doc and         -->
  <!--                       pass the result to this style sheet residing   -->
  <!--                       in that directory. This overrides              -->
  <!--                       contextXsltFile and globalXsltFile[null]       -->
  <!--                                                                      -->
  <!--   contextXsltFile     Make directory listings an XML doc and         -->
  <!--                       pass the result to this style sheet which is   -->
  <!--                       relative to the context root. This overrides   -->
  <!--                       globalXsltFile[null]                           -->
  <!--                                                                      -->
  <!--   globalXsltFile      Site wide configuration version of             -->
  <!--                       localXsltFile. This argument must either be an -->
  <!--                       absolute or relative (to either                -->
  <!--                       $CATALINA_BASE/conf or $CATALINA_HOME/conf)    -->
  <!--                       path that points to a location below either    -->
  <!--                       $CATALINA_BASE/conf (checked first) or         -->
  <!--                       $CATALINA_HOME/conf (checked second).[null]    -->
  <!--                                                                      -->
  <!--   showServerInfo      Should server information be presented in the  -->
  <!--                       response sent to clients when directory        -->
  <!--                       listings is enabled? [true]                    -->