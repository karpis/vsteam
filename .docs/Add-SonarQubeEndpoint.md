#include "./common/header.md"

# Add-VSTeamSonarQubeEndpoint

## SYNOPSIS
#include "./synopsis/Add-VSTeamSonarQubeEndpoint.md"

## SYNTAX

### Secure (Default)
```
Add-VSTeamSonarQubeEndpoint [-ProjectName] <String> [-SecurePersonalAccessToken] <SecureString> [-SonarQubeUrl] <String>
 [[-EndpointName] <String>]
```

### Plain
```
Add-VSTeamSonarQubeEndpoint [-ProjectName] <String> [-PersonalAccessToken] <String> [-SonarQubeUrl] <String>
 [[-EndpointName] <String>]
```

## DESCRIPTION
The cmdlet adds a new connection between TFS/VSTS and a SonarQube server using
the SonarQube connection type. 

This is only used when using the SonarQube tasks.

Using SonarQube with the Maven tasks uses a Generic Connection type.

## EXAMPLES

## PARAMETERS

### -SonarQubeUrl
URL of the sonarqube server.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PersonalAccessToken
Authentication Token generated by SonarQube.

```yaml
Type: String
Parameter Sets: Plain
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EndpointName
The name displayed on the services page. 
In VSTS this is the Connection Name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```


### -SecurePersonalAccessToken
A secured string to capture your personal access token. 

This will allow you to provide your personal access token
without displaying it in plain text.

To use pat simply omit it from the Add-VSTeamAccount command.

```yaml
Type: SecureString
Parameter Sets: Secure (Default)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

#include "./params/projectName.md"

## INPUTS

### System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

