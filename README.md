# XKB-Windows-Persian-Configuration

X keyboard "Microsoft windows Persian layout" configuration 



This is a Persian keyboard layout for the people who want to use their windows layout in the Debian based Linux


# install


1) `git clone https://github.com/SeniorHunter/xkb-windows-persian-configuration.git`

2) `cd xkb-windows-persian-configuration/`

3) `sudo mv ir /usr/share/X11/xkb/symbols/`


4) open `/usr/share/X11/xkb/rules/evdev.xml` and look for Persian language part

```
<layout>
	<configItem>
		<name>ir</name>
		<shortDescription>fa</shortDescription>
		<description>Persian</description>
		<languageList>
			<iso639Id>per</iso639Id>
		</languageList>
	</configItem>

	<variantList>
		...
		{your code}
		...
	</variantList>
</layout>
```  

5) you have to add this part of code inside the layout:variantList block (it is a variant block)

```
<variant>
	<configItem>
		<name>pes_windows</name>
		<description>Persian (windows)</description>
	</configItem>
</variant>
 ```
