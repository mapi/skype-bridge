﻿SkypeIrcGateway
============

SkypeとIRCをつなぐゲートウェイ

===================== ========================================
ファイル              概要
===================== ========================================
sig.cmd               sig.jsを起動するコマンドファイル
sig.js                sig.rbを死活監視するJScript
sig.rb                SkypeとIRCのゲートウェイ
lib/skype_client.rb   Skypeのインターフェイス
lib/irc_client.rb     IRCのインターフェイス
lib/twitter_client.rb Twitterのインターフェイス
t2s.rb                TwitterからSkypeにメッセージを流すボット
===================== ========================================

対象
----

- Windows専用

  - Ruby4Skypeに依存

- Skype APIを使うためSkypeの起動が必要

使用方法
--------

::

  > gem install pit
  > gem install Ruby4Skype
  > set EDITOR=notepad
  > ruby sig.rb [pit-suffix]

予定
----

- stg.rb
 
  - SkypeとTwitterのゲートウェイ

- t2s.rb
  
  - TwitterからSkypeへの通知

制限事項
--------

Ruby4Skypeの仕様だと思うのですが、シグナルのトラップが無効になるため、強制終了しなければ終了できません

参照
----

- Ruby4Skype

  - http://rubyforge.org/projects/skyperapper

  - http://skyperapper.rubyforge.org/

