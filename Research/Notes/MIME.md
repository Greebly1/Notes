Multipurpose Internet Mail Extension
A translation layer that encapsulates [[SMTP]] mail that allows encoding extra information within an email not previously possible.

# Extensions
Allows sending of different file extensions, such as png, jpeg, webm, audio files, video, etc.

# Binary Data
Can send raw binary data of unsupported file types.

# Extra languages
Languages with extra letters, such as Chinese, Arabic, etc, can be sent.
This is due to SMTPs dependency on the 7 bit ASCII symbols. It isn't enough to encode the symbols of other languages.

# Header
Mail that uses MIME, is wrapped in a MIME header. 

MIME-Version: 1.0
Content-Type: text/plain or image/jpeg or audio/mp3 etc
Content-Disposition: attachment; filename=genome.jpeg;
  modification-date="Wed, 12 Feb 1997 16:29:51 -0500";
Content-Transfer-Encoding: base64

These headers allow the receiver to determine how to parse the mail data.