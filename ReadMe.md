# GitHub Repositories
[Joschua Glau/BibleGateway-to-Obsidian](https://github.com/selfire1/BibleGateway-to-Obsidian) - Download the release files

[Jonathan Clark/BibleGateway-to-Markdown](https://github.com/jgclark/BibleGateway-to-Markdown) - Download and copy only "bg2md.rb" to the same folder

# Install 
### Ruby
https://rubyinstaller.org/downloads/

### Install RubyGem components as per [Jonathan Clark](https://github.com/jgclark/BibleGateway-to-Markdown#installation)
These can be run in any terminal
```ruby
gem update --system
```

```ruby
gem colorize optparse clipboard
```

### Install Git Bash
https://git-scm.com/
<img width="1257" height="887" alt="image" src="https://github.com/user-attachments/assets/531309fa-3cb5-4b23-b8c1-f552d44588bf" />

# Bash Terminal
### Check 1
Run commands-
```bash
ruby -v
which ruby
```
If second command `which ruby` is not working follow the steps below.

### Check which bash is being used
```powershell
Get-Command bash
```
If "C:\WINDOWS\system32\bash.exe" is shown it suggests WSL (Windows Subsystem for Linux) not Git Bash. **You need to be on Git Bash.**

If "C:\Program Files\Git\bin\bash.exe" is shown it is Git Bash and you can directly start running the commands `bg2obs.sh -i -v NET`

**Solution 1**

Open "Git Bash". Use Windows search (Git Bash) or "C:\Program Files\Git\git-bash.exe".
<img width="942" height="622" alt="image" src="https://github.com/user-attachments/assets/000ee307-d0c0-45a2-b480-4cb2504854c4" />

```
bash bg2obs.sh -i -v NET
```
**Solution 2**
```bash
& "C:\Program Files\Git\bin\bash.exe" bg2obs.sh -i -v NET
```

# Try if all fails
### Fix 1 - Perl Strawberry
Install Perl Strawberry (use any 1)

https://www.perl.org/get.html

or

https://github.com/StrawberryPerl/Perl-Dist-Strawberry

or
```powershell
winget install --id StrawberryPerl.StrawberryPerl -e --source winget
```

### Fix 2 - As per [discussion](https://forum.obsidian.md/t/bible-study-kit-in-obsidian-scripts-help-and-support/31069/15), if it doesn't work try
```ruby
gem ffi
```
# Additional
### [If you ever want to uninstall Ruby, remove installed gem first](https://stackoverflow.com/a/49960935)
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
