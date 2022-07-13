# Areia_Align_Lock
Automatically lock align

## Overview
This is meant for players who have access to an align lock clanskill like Apathy. If you are not a member of a clan with this sort of cskill, this will proove useless to you.

### Setup
By default, settings are configured to assume the use of Pyre's clanskill. If you are a member of a different clan, or if Pyre's clanskill messages have changed, do the following to get started once you have downloaded and installed the script:

1. Set the cskill's name
   * This is the command you would type to use the skill (e.g., 'apathy').
   * For example, *aal config cskillcmd l33tcskillname*.
2. Set the cskill's success message.
   * This is the message seen when the cskill is successfully cast.
   * For example, *aal config cskillon Your align is now locked. L33t!*.
3. Set the cskill's fail message.
   * This is the message you see when the cskill is not active and you try but fail to cast it.
   * For example, *aal config cskillfail You fail to invoke the power of l33tdom. U r teh sux0rz.*.
4. Set the cskill's expire message.
   * This is the message you see when the cskill's duration hits 0.
   * For example, *Oh nyo, your align is no longer locked. Halp!*.

Note that all of these messages are given in plain text. You do not need to write regular expressions or anything of that kind. Simply copy and paste your cskill's messages with the plugin commands, and you'll be good to go.

## Main Plugin Commands
aal help [<topic>]: Display plugin's help topics.

aal config auto [on|off]: Set/toggle whether the plugin automatically tries to lock your alignment when your cskill drops or fails to cast.

aal config align [good|neutral|evil]: Set/cycle through the alignment into which you want to be locked. If this does not match your current align, the plugin will not auto-lock.

aal config cskillon [<message>]: Set the message seen when your cskill casts successfully.

aal config cskilloff [<message>]: Set the message seen when your cskill expires.

aal config cskillfail [<message>]: Set the message seen when your cskill fails.

aal config cskillcmd [<cmd>]: Set the command used to cast your cskill.
