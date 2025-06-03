 # Swirl Lesson 1: Workspace and Files
**Completed on:** June 3, 2025  
**Platform:** Windows (R version 4.5.0)  
**Course:** R Programming  
**Lesson:** Workspace and Files  
**Tool Used:** swirl

---

## 🌐 Session Info

```r
R version 4.5.0 (2025-04-11 ucrt) -- "How About a Twenty-Six"
Platform: x86_64-w64-mingw32/x64
# Check working directory
getwd()

# List variables in the workspace
ls()

# Assign variable
x <- 9

# List files in the working directory
list.files()

# View help documentation
?list.files

# View function arguments
args(list.files)

# Store working directory
old.dir <- getwd()

# Create directory
dir.create("testdir")

# Change working directory
setwd("testdir")

# Create a file
file.create("mytest.R")

# Check if file exists
file.exists("mytest.R")

# Get file metadata
file.info("mytest.R")

# Rename a file
file.rename("mytest.R", "mytest2.R")

# Copy a file
file.copy("mytest2.R", "mytest3.R")

# Construct file paths
file.path("folder1", "folder2")

# Create nested directories
dir.create(file.path("testdir2", "testdir3"), recursive = TRUE)

# Return to original working directory
setwd(old.dir)
