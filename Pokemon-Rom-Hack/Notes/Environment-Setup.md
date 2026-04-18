# Environment Setup

## Structure

Local development environment is organized as follows:

- Emulator: VBA-M for running ROMs  
- Tools: Advance Map, Hex Maniac Advanced  
- ROM: Clean and working ROM files  
- Resources: Original downloaded files  
- Decomp: pokeemerald source repository  
- Terminal: MSYS2 (UCRT64 environment)

---

## ROM Setup

- Pokémon Emerald (v1.0)  
- Pokémon FireRed (v1.0)  

Working copies are created for editing while keeping clean ROMs unchanged.

---

## Tool Setup

### Legacy Tools
- Advance Map  
- Advance Text  

### Hybrid Tools
- Hex Maniac Advanced  

### Decomp Tools
- pokeemerald (pret)

---

## MSYS2 Environment

### Terminal
- Using **UCRT64** for all development work  

### System Update
Commands:
pacman -Syu  
pacman -Su  

---

### Build Tools
Installed:
pacman -S make mingw-w64-ucrt-x86_64-toolchain  

Includes:
- gcc  
- g++  
- make  

---

### Dependencies
Installed:
pacman -S mingw-w64-ucrt-x86_64-libpng mingw-w64-ucrt-x86_64-zlib pkgconf  

Purpose:
- libpng → graphics processing  
- zlib → compression  
- pkgconf → dependency management  

---

### ARM Toolchain
Installed:
pacman -S mingw-w64-ucrt-x86_64-arm-none-eabi-toolchain  

Includes:
- arm-none-eabi-gcc  
- binutils  
- newlib  

Purpose:
- Compile code for Game Boy Advance  

---

### Git Setup
Installed:
pacman -S git  

Purpose:
- Repository management inside MSYS2  

---

## Workflow

- Edit ROM using Advance Map / Hex Maniac Advanced  
- Test using VBA-M emulator  
- Use decomp tools for advanced development  
- Maintain version control for all changes  

---

## Goal

To maintain a clean, structured, and scalable environment for ROM hacking from basic editing to advanced development.
