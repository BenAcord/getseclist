# getseclist
Display the line counts for various word lists based on a keyword search.

Helpful for determining the best list for fuzzing a given target (eg. DirB, Gobuster, DirBuster, wfuzz, etc.)

USAGE	./getseclist -k keyword
  
  WHERE	keyword   - a word to check seclist titles
  
  EXAMPLE	./getseclist -k rockyou

---

## Examples
Directory options
```bash
example $ ./getseclist -k dir
[*]  getseclist
[*]  Checking: /usr/share/seclists/ /usr/share/wordlists/

LineCount  Filepath
---------  -----------------------------------------------
220560     /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
207643     /usr/share/wordlists/dirbuster/directory-list-lowercase-2.3-medium.txt
141708     /usr/share/wordlists/dirbuster/directory-list-1.0.txt
87664      /usr/share/wordlists/dirbuster/directory-list-2.3-small.txt
81643      /usr/share/wordlists/dirbuster/directory-list-lowercase-2.3-small.txt
62290      /usr/share/seclists/Discovery/Web-Content/raft-large-directories.txt
58688      /usr/share/wordlists/dirbuster/directories.jbrofuzz
56180      /usr/share/seclists/Discovery/Web-Content/raft-large-directories-lowercase.txt
30009      /usr/share/seclists/Discovery/Web-Content/raft-medium-directories.txt
26593      /usr/share/seclists/Discovery/Web-Content/raft-medium-directories-lowercase.txt
20122      /usr/share/seclists/Discovery/Web-Content/raft-small-directories.txt
17776      /usr/share/seclists/Discovery/Web-Content/raft-small-directories-lowercase.txt
5967       /usr/share/seclists/Discovery/Web-Content/SVNDigger/all-dirs.txt
2346       /usr/share/seclists/Discovery/Web-Content/KitchensinkDirectories.fuzz.txt
855        /usr/share/wordlists/wfuzz/vulns/dirTraversal.txt
847        /usr/share/wordlists/wfuzz/vulns/dirTraversal-win.txt
847        /usr/share/wordlists/wfuzz/vulns/dirTraversal-nix.txt
67         /usr/share/seclists/Discovery/Web-Content/domino-dirs-coldfusion39.txt
48         /usr/share/wordlists/wfuzz/webservices/ws-dirs.txt
13         /usr/share/seclists/Discovery/Web-Content/default-web-root-directory-linux.txt
3          /usr/share/seclists/Discovery/Web-Content/default-web-root-directory-windows.txt

```
Files for fuzzing
```
example $ ./getseclist -k files
[*]  getseclist
[*]  Checking: /usr/share/seclists/ /usr/share/wordlists/

LineCount  Filepath
---------  -----------------------------------------------
37042      /usr/share/seclists/Discovery/Web-Content/raft-large-files.txt
35324      /usr/share/seclists/Discovery/Web-Content/raft-large-files-lowercase.txt
17128      /usr/share/seclists/Discovery/Web-Content/raft-medium-files.txt
16243      /usr/share/seclists/Discovery/Web-Content/raft-medium-files-lowercase.txt
11424      /usr/share/seclists/Discovery/Web-Content/raft-small-files.txt
10848      /usr/share/seclists/Discovery/Web-Content/raft-small-files-lowercase.txt
116        /usr/share/seclists/Discovery/Web-Content/Domino-Hunter/Domino_Files.txt
48         /usr/share/seclists/IOCs/kaspersky-careto-files.txt
48         /usr/share/seclists/IOCs/kaspersky-careto-files-no-env-vars.txt
39         /usr/share/seclists/Discovery/Web-Content/UnixDotfiles.fuzz.txt
24         /usr/share/seclists/Discovery/Web-Content/Randomfiles.fuzz.txt
19         /usr/share/wordlists/wfuzz/webservices/ws-files.txt
16         /usr/share/wordlists/metasploit/sensitive_files.txt
7          /usr/share/wordlists/metasploit/sensitive_files_win.txt
3          /usr/share/seclists/Fuzzing/MySQL-Read-Local-Files.fuzzdb.txt
```

Specific application
```
example $ ./getseclist -k apache
[*]  getseclist
[*]  Checking: /usr/share/seclists/ /usr/share/wordlists/

LineCount  Filepath
---------  -----------------------------------------------
10355      /usr/share/wordlists/dirbuster/apache-user-enum-2.0.txt
8930       /usr/share/wordlists/dirbuster/apache-user-enum-1.0.txt
8531       /usr/share/seclists/Discovery/Web-Content/Apache.fuzz.txt
53         /usr/share/seclists/Discovery/Web-Content/ApacheTomcat.fuzz.txt
31         /usr/share/seclists/Discovery/Web-Content/apache.txt
30         /usr/share/wordlists/wfuzz/vulns/apache.txt
30         /usr/share/wordlists/dirb/vulns/apache.txt
```
