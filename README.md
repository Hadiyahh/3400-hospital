# Hospital Management System

A command-line hospital management system developed as a team project for COMP-3400.

The application manages core hospital operations including patients, doctors, nurses, pharmacy workflows, and hospital records using C/C++ and SQLite.

## My Contributions

I was responsible for the **Pharmacy** and **Nurse** modules, including the logic and workflows associated with those parts of the system.

## Features

- Patient management
- Doctor management
- Nurse management
- Pharmacy management
- Hospital record management
- SQLite-backed persistence
- Modular C/C++ architecture

## Build & Run

To run in codespace:
```
g++ src/mainmenu.cpp src/modules/*.cpp SQLiteCpp/src/*.cpp -o hospitalSystem -I SQLiteCpp/include -I src/include -lsqlite3
```

If that doesnt work, try:
```
g++ src/mainmenu.cpp src/modules/*.cpp SQLiteCpp/src/*.cpp -o hospitalSystem -I SQLiteCpp/include -I src/include -lsqlite3
```

Then :
```
./hospitalSystem
```

### Debian (WSL)
Note: The paths to the SQL files may be incorrect when running locally (to support running in Codespaces). Change the paths in `database.cpp` from `/sql` to `../sql`.
#### Requirements
- gcc v12.x
- Cmake
#### Build
In the root folder, run `build.sh`
#### Run
In `/build`, run `hms`. The database SQLite file will be create in `/build` as `hms.db3`.

## Presentation Slides:
https://www.canva.com/design/DAGjCmUITMA/quZPshsPzRhmDX8a_TUUfg/edit?utm_content=DAGjCmUITMA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
