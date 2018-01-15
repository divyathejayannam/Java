# Java
Java Basics 
import java.io.IOException;
import java.io.InputStream;
import java.io.BufferedReader;
import java.io.PrintWriter;
import java.io.InputStreamReader;
import java.util.Enumeration;
import java.util.Iterator;
import java.util.zip.ZipEntry;
import java.util.zip.ZipFile;
import com.redwood.scheduler.api.model.*;
import com.redwood.scheduler.api.model.enumeration.*;
import com.redwood.scheduler.api.date.*;
import java.util.Date;
import java.text.SimpleDateFormat;
{  
    Table tbl =  jcsSession.getTableByName("PHL_JOB_LIST");
 
    java.util.HashSet keys = new java.util.HashSet();
    for (Iterator it = tbl.getTableValues(); it.hasNext(); ) 
    {
      TableValue tv = (TableValue)it.next();
      keys.add(tv.getKey());
    }
