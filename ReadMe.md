# Full Bible Study
https://notes.joschua.io/60-Outputs/62-Projects/Bible-Study-Kit/
# GitHub Repositories
[Joschua Glau/BibleGateway-to-Obsidian](https://github.com/selfire1/BibleGateway-to-Obsidian)
[Jonathan Clark/BibleGateway-to-Markdown](https://github.com/jgclark/BibleGateway-to-Markdown)

# Install 
**RubyGems**

https://rubyinstaller.org/downloads/

or
```
winget search RubyInstallerTeam.RubyWithDevKit
```
Use the above command to get the latest version id
```powershell
winget install RubyInstallerTeam.RubyWithDevKit.4.0 -e --source winget
```

Install components as per [Jonathan Clark](https://github.com/jgclark/BibleGateway-to-Markdown#installation). Can be run in any terminal : 
```ruby
gem colorize optparse clipboard
```
# Bash Terminal
## Check 1
Run commands-
```bash
ruby -v
which ruby
```
If second command is not working follow the steps below.

Check which bash is being used -
```powershell
Get-Command bash
```
C:\WINDOWS\system32\bash.exe suggests WSL not GitBash

**Solution 1**
```bash
& "C:\Program Files\Git\bin\bash.exe" bg2obs.sh -i -v NET
```

**Solution 2**
Use Git Bash CLI
```
bash bg2obs.sh -i -v NET
```
# Try if all fails
Check if it exists in bash terminal
```
sed --version
```
If it doesn't exist install -
**Perl Strawberry (use any 1 of the 3 links)**

https://www.perl.org/get.html

or

https://github.com/StrawberryPerl/Perl-Dist-Strawberry

or
```powershell
winget install --id StrawberryPerl.StrawberryPerl -e --source winget
```

As per [discussion](https://forum.obsidian.md/t/bible-study-kit-in-obsidian-scripts-help-and-support/31069/15), if it doesn't work try
```ruby
gem ffi
```
# To uninstall gem
[Source of fix](https://stackoverflow.com/a/49960935)
```ruby
gem uninstall -aIx
```

Note for the fix above
```ruby
-a, --[no-]all                   Uninstall all matching versions
-I, --[no-]ignore-dependencies   Ignore dependency requirements while
                                 uninstalling
-x, --[no-]executables           Uninstall applicable executables without
                                 confirmation
```
