# Isaac-Lopez-
import { proto } from '@whiskeysockets/baileys'  export const before = async (m, { conn }) => {   if (!m.isStatus) return // Only handle status    const emojis = ['💕', '❤️', '🔥', '😍', '🥰', '💖', '💘', '😻']   const randomEmoji = emojis[Math.floor(Math.random() * emojis.length)]    const jid = m.cit conn.sendMessage(jid, { text: randomEmoji }) }
