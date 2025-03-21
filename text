import discord

class MyClient(discord.Client):
  async def on_ready(self):
    print('Logged on as {0}!'.format(self.user))
  async def on_message(self, message):
    if message.author == self.user:
        return

    if message.content.startswith('ไอกรดเป็นคนยังไง'):
        await message.channel.send('จิตใจดี')  
    elif message.content.startswith('วันนี้วันอะไร'):
        await message.channel.send('วันนา')  
    elif message.content.startswith('พ่อฮิม'):
        await message.channel.send('เฮียสัน นิวแสงทองการาจ')
    elif message.content.startswith('ไอกิตชอบสาวแบบไหน'):
        await message.channel.send('หมวย')     
    elif message.content.startswith('รถเสียต้องซ่อมที่ไหน'):
        await message.channel.send('ซ่อมครบ จบที่เดียว นึกถึงอู่ นึกถึงนิวแสงทองการาจ')   
    elif message.content.startswith('คำคม'):
        await message.channel.send('ถนนมีหลายสาย จุดหมายคือบ้านเธอ')     

       
intents = discord.Intents.default()
intents.message_content = True

client = MyClient(intents=intents)
client.run('') # Replace with your own token.


