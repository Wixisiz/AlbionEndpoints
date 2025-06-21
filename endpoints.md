# Base URL
https://gameinfo.albiononline.com/api/gameinfo/


# GET /players/{playerId}
Contains general data on player
| NAME                  | DATA TYPE |                     DESCRIPTION                   
|-----------------------|-----------|---------------------------------------------------
| Name                  | string    |   Player's in-game name                           
| Id                    | string    |   Player ID                                       
| GuildName             | string    |   Player's guild (May be excluded)                
| GuildId               | string    |   Guild ID (May be excluded)                      
| AllianceName          | string    |   Player's alliance (May be excluded)             
| AllianceId            | string    |   Alliance ID (May be excluded)                   
| AllianceTag           | string    |   Alliance tag (May be excluded)                  
| Avatar                | string    |   Name of player profile avatar                   
| AvatarRing            | string    |   Name of player profile avatar ring              
| DeathFame             | int       |   Total fame given due to deaths                  
| KillFame              | int       |   Total game from kills                           
| FameRatio             | long      |   KillFame / DeathFame                            
| LifetimeStatistics    | object    |   Contains extensive details on PVE fame          


# GET /players/{playerId}/kills
Contains data on last 10 kills of player
# GET /players/{playerId}/deaths
Contains data on last 10 deaths of player

| NAME                  | DATA TYPE |                     DESCRIPTION                   
|-----------------------|-----------|---------------------------------------------------
| numberOfParticipants  | int       |   Total number of contributers including killer                     
| groupMemberCount      | int       |   Players in player's party                                                            
| EventId               | int       |   Event ID    
| TimeStamp             | string    |   Exact time kill occured                                              
| Version               | int       |                  ???                                                      
| Killer                | Object    |   Contains information about equipment of killer and average item power   
| Player Information    | Object    |   Same structure as in ['/players/{playerId}']        
| Victim                | Object    |   Contains information about equipment of victim and average item power                   
| TotalVictimKillFame   | int       |   Total fame recieved by killer and contributers    
| Participants          | object    |   Contains information about contributers including killer                 
| FameRatio             | long      |   KillFame / DeathFame                            
| LifetimeStatistics    | object    |   Contains extensive details on PVE fame
| BattleId              | int       |   Battle ID (different from Event ID)
| KillArea"             | string    |   Type of location where kill occured


# GET /players/{playerId}
# GET /players/{playerId}
# GET /players/{playerId}

# /search?q={name}
# /items/_weaponCategories
