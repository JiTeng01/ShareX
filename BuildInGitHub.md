****Build Requirement****
1. MSBuild 15.0 or above
2. Nuget package
3. Git Bash

####Build Step####

#1 Clone the ShareX into local directory.
git clone https://github.com/JiTeng01/ShareX.git

#2 export the MSBuild.exe directory enviroment
export PATH=$PATH:/c/Program\ Files\ \(x86\)/Microsoft\ Visual\ Studio/2017/Community/MSBuild/15.0/Bin/

#3 export the Nuget.exe directory
export PATH=$PATH:/d/SCC_Project/ShareX/.nuget/

#4 update the nuget to latest version
NuGet.exe update -self

#5 usie the nuget to restore ShareX.sln
NuGet.exe restore ShareX.sln

#6 Build ShareX using MsBuild
MSBuild.exe ShareX.sln