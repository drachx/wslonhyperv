# wsl on hyperv

1. Set-VMProcessor -VMName <VMName> -ExposeVirtualizationExtensions $true
2. Reboot host
3. Login to VM
4. Install WSL
5. Enable HyperV from Windows Features (Add/Remove Programs)
6. You might need to reboot the VM
7. Launch Windows Security > App & Browser Control > Exploit Protection > Program Settings > add C:/windows/system32/VMCompute > Control Flow Guard ticked
8. Reboot VM
9. wsl --set-default-version 2
10. wsl --install Ubuntu (--beb-download if you are stuck at 0%)
