<h1 align="center">Using GitHub Packages for publishing NuGet packages</h1>

<p align="center">
  <a href="#mega-prerequisites">Prerequisites</a> •  
  <a href="#books-resources">Resources</a>
</p>

This repository can be used as a reference guide/sample to enable publishing your first package via Github Container Registry.

## :mega: Prerequisites

- A [GitHub.com account](https://github.com/join) with a [verified e-mail address](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/verifying-your-email-address)
- Basic understanding of `yaml` syntax
- Basic understanding of DevOps processes
- Basic understanding of software package registries (e.g. GitHub Packages, nuget)
- Nice to have: experience with GitHub Actions or other automation servers such as Jenkins or TravisCI

## Publishing a package using a nuget.config file

When publishing, you need to use the same value for OWNER in your csproj file that you use in your nuget.config authentication file. Specify or increment the version number in your .csproj file, then use the dotnet pack command to create a .nuspec file for that version. 

## Installing a package
Using packages from GitHub in your project is similar to using packages from nuget.org. Add your package dependencies to your .csproj file, specifying the package name and version. 

## :books: Resources

- [Introduction to YAML: Learn YAML in 5 minutes](https://www.codeproject.com/Articles/1214409/Learn-YAML-in-five-minutes)
- [GitHub Docs: GitHub Actions](https://docs.github.com/actions)
- [GitHub Docs: Workflow syntax](https://docs.github.com/actions/reference/workflow-syntax-for-github-actions)
- [GitHub Docs: REST API](https://docs.github.com/rest)
- [GitHub Docs: GraphQL API](https://docs.github.com/graphql)
- [GitHub Docs: GitHub Packages: NuGet](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-nuget-registry)
