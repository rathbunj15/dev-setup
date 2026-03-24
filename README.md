# dev-setup
This repository contains scripts and playbooks for configuring and installing the tools required for programming. 


## Installed Tools
The following items are installed when running the `dev-setup` script.

<strong>Required</strong>
<ul>
    <li>Python 3.12 (with pip3)</li>
    <li>Ansible</li>
</ul>
<strong>Custom Scripts</strong>
<ul>
    <li><code>gitp</code> <i>(located at <a href=bin/gitp>bin/gitp</a>)</i>
        <ul>
            <li>A utility script for fast git operations</li>
        </ul>
    </li>
    <li><code>mkscript</code> <i>(located at <a href=bin/mkscript>bin/mkscript</a>)</i>
        <ul>
            <li>A utility script for creating scripts that are pre-configured for executable permissions.</li>
        </ul>
    </li>
</ul>
<strong>Packages</strong>
<ul>
    <li><code>ansible-lint</code></li>
    <li><code>zip</code></li>
    <li><code>unzip</code></li>
    <li><code>wget</code></li>
    <li><code>curl</code></li>
    <li><code>git</code></li>
    <li><code>make</code></li>
    <li><code>jq</code></li>
    <li><code>jid</code></li>
    <li><code>screen</code></li>
    <li><code>oc</code></li>
    <li><code>helm</code></li>
</ul>
<strong>Aliases</strong>
<table>
    <thead>
        <tr>
            <th>Alias</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>lsa</code></td>
            <td>An alias for <i>ls -lat</i></td>
        </tr>
        <tr>
            <td><code>dps</code></td>
            <td>Lists all running docker containers</td>
        </tr>
        <tr>
            <td><code>di</code></td>
            <td>Lists all docker images on the local docker repository</td><tr>
        <tr>
            <td><code>dstop</code></td>
            <td>Stops all running docker containers</td></tr>
        <tr>
            <td><code>drm</code></td>
            <td>Stops and removes all running docker containers</td></tr>
        <tr>
            <td><code>drmi</code></td>
            <td>Removes all docker images currently in the local docker registry</td></tr>
        <tr>
            <td><code>dboom</code></td>
            <td>Destroys all docker containers, images, volumes, and netw
            orks.</td></tr>
        <tr>
            <td><code>dexec</code></td>
            <td>Executes a command in a docker container (in interactive mode)</td></tr>
        <tr>
            <td><code>dbash [container]</code></td>
            <td>Enters a bash in the supplied container</td></tr>
        <tr>
            <td><code>dcu</code></td>
            <td>Runs docker-compose up</td></tr>
        <tr>
            <td><code>dcd</code></td>
            <td>Runs docker-compose down</td></tr>
        <tr>
            <td><code>dprune</code></td>
            <td>Prunes all system volumes</td></tr>
    </tbody>
</table>

## Repository structure
<ul>
    <li> 
        <code>bin</code>
        <ul>
            <li>Contains scripts that are ready to be copied to the host system.</li>
        </ul>
    </li>
    <li>
        <code>playbooks</code>
        <ul>
            <li>Contains Ansible playbooks for installing the scripts and other tools.</li>
        </ul>
    </li>
</ul>
