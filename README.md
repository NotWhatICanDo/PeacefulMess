# PeacefulMess

    in_thread do
    22.times do
    play sample :guit_harmonics
    sleep 1
    play sample :guit_e_fifths
    sleep 1.1
    play sample :guit_e_slide
    sleep 1.2
    play sample :guit_em9
    sleep 0.4
     end
    end

    in_thread do
     5.times do
    sample :drum_heavy_kick
    sleep 0.25
    end
  
    1.times do
    play_pattern chord(:E3, :m7)
    play_pattern_timed chord(:E3, :m7), 0.25
    play_pattern_timed chord(:E3, :m13), [0.25, 0.5]
     end
  
     sleep 0.5
  
  
    3.times  do
    sample :guit_em9
    play 21
    sample :guit_e_fifths
    sleep 5
    sample :guit_em9
     end
    sample :guit_harmonics
  
    sleep 1
  
    5.times do
    sample :drum_heavy_kick
    sleep 0.25
     end
  
  
     live_loop:nom do
    cue 'guitar9'
    key = cue 'guitar'
    3.times do
      3.times do
        live_loop :drums do
          sample :drum_heavy_kick
          sleep 0.25
        end
      end
      
      live_loop :hihat do
        sample :drum_cymbal_pedal
        sleep 0.50
        sample :drum_cymbal_pedal
        sleep 0.75
      end
    end
    
    live_loop :algo do
      sample :drum_snare_hard
      sleep 1
    end
    end
  
  
  
     3.times  do
    sample :guit_em9
    play 21
    sample :guit_e_fifths
    sleep 5
    sample :guit_em9
     end
     sample :guit_harmonics
  
     sleep 2
  
     play 70, amp: 0.5, attack: 0.5, sustain: 1
     play 55, amp: 0.5, attack: 0.5, sustain: 1
  
    sleep 0.5
  
    2.times do
    key = cue 'guitar9'
    use_synth :pluck
    with_fx :level do
      play 70, amp: 2, sustain: 1
      play 55, amp: 2, sustain: 1
      sleep 0.5
      play 70, amp: 2, sustain: 1
      play 55, amp: 2, sustain: 1
      sleep 0.5
      play 70, amp: 2, sustain: 1
      play 55, amp: 2, sustain: 1
      sleep 0.5
      play 75, amp: 2, sustain: 1
      play 60, amp: 2, sustain: 1
      sleep 0.5
      play 75, amp: 2, sustain: 1
      play 60, amp: 2, sustain: 1
      sleep 0.5
      play 75, amp: 1.5, sustain: 1
      play 60, amp: 1.5, sustain: 1
      sleep 0.5
      play 65, amp: 1.5, sustain: 1
      play 50, amp: 1.5, sustain: 1
      sleep 0.5
      play 65, amp: 1.5, sustain: 1
      play 50, amp: 1.5, sustain: 1
      sleep 0.5
      play 65, amp: 1.5, sustain: 1
      play 50, amp: 1.5, sustain: 1
      sleep 0.5
    end
    end
  
     3.times do
    key = cue 'guitar9'
    use_synth :pluck
    with_fx :level do
      with_fx :echo do
        play 70, amp: 3, sustain: 1
        play 55, amp: 3, sustain: 1
        sleep 0.5
        play 70, amp: 2, sustain: 1
        play 55, amp: 2, sustain: 1
        sleep 0.5
        play 70, amp: 2, sustain: 1
        play 55, amp: 2, sustain: 1
        sleep 0.5
        play 75, amp: 2, sustain: 1
        play 60, amp: 2, sustain: 1
        sleep 0.5
        play 75, amp: 2, sustain: 1
        play 60, amp: 2, sustain: 1
        sleep 0.5
        play 75, amp: 1.5, sustain: 1
        play 60, amp: 1.5, sustain: 1
        sleep 0.5
        play 65, amp: 1.5, sustain: 1
        play 50, amp: 1.5, sustain: 1
        sleep 0.5
        play 65, amp: 1.5, sustain: 1
        play 50, amp: 1.5, sustain: 1
        sleep 0.5
        play 65, amp: 1.5, sustain: 1
        play 50, amp: 1.5, sustain: 1
        sleep 0.5
      end
    end
     end
    end
