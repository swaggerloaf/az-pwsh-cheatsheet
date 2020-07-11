# az-pwsh-cheatsheet

<code>$PSVersionTable.PSVersion</code>

<code>Connect-AzAccount</code>

<code>$PSVersionTable.PSVersion</code>

<code>if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Force
}
  </code>

<code>Get-InstalledModule -Name Az -AllVersions</code>

<code>Import-Module -Name Az -RequiredVersion 4.3.0</code>

<code>Get-Command -Verb Get -Noun AzVM* -Module Az.Compute</code>

<code>Get-Command -Verb Get -Noun Az* -Module Az.Network</code>
