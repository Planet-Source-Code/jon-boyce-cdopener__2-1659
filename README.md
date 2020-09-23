<div align="center">

## Cdopener


</div>

### Description

Opens and closes a cd tray
 
### More Info
 
This code is actually visual j++ the package com.ms.win32 is not part of the java api and is not standard sun code.!!!!!!!!!!

You need a very up to date virual machine to interpret the java bytecode otherwise the code will not work, ie5 has a very good up to date virtual machine, i highly recomend this as it will make life a lot easier


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jon Boyce](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jon-boyce.md)
**Level**          |Unknown
**User Rating**    |4.5 (18 globes from 4 users)
**Compatibility**  |Java \(JDK 1\.1\)
**Category**       |[Windows](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows__2-80.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jon-boyce-cdopener__2-1659/archive/master.zip)





### Source Code

```
import com.ms.win32.*;
public class Cdopener
{
	private static String OPEN = "set cdaudio door open";
	private static String CLOSE = "set cdaudio door open";
	private static final int MAX_ERROR_SIZE = 64;
	private static StringBuffer sbreturn = new StringBuffer(MAX_ERROR_SIZE);
	public static void main (String[] args)
	{
		//call open() to open it and close() in the main method to
        //close it
	}
	public static void open()
	{
	 Winmm.mciSendString(OPEN,sbreturn,127,0);
	}
	public static void close()
	{
	 Winmm.mciSendString(CLOSE,sbreturn,127,0);
	}
}
```

