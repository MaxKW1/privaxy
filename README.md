
## Installation

cd web_frontend
npm i
trunk build --release
cd ..
cd privaxy
cargo build --release --all-targets
cd ..
cargo build --release --all-targets


Go to the GUI, click on "Save CA certificate".
cp privaxy_ca_cert.pem /usr/local/share/ca-certificates/

Configure your local system to pass http traffic through privaxy which listens on 0.0.0.0:8100
   - Macos: <https://support.apple.com/guide/mac-help/change-proxy-settings-network-preferences-mac-mchlp2591/mac>
   - Ubuntu (gnome): <https://phoenixnap.com/kb/ubuntu-proxy-settings>
